# Teste Prático - Desenvolvedor Frontend Vue.js

## 📋 Descrição do Projeto

Desenvolver uma **Progressive Web App (PWA)** utilizando Vue.js para um sistema de vendas simples. O projeto deve demonstrar conhecimentos em Vue.js, Vue Router, gerenciamento de estado e desenvolvimento de PWA.

## 🎯 Objetivos do Teste

- Implementar uma PWA funcional com Vue.js
- Utilizar Vue Router para navegação entre páginas
- Implementar gerenciamento de estado (Vuex/Pinia)
- Criar interface responsiva e moderna
- Demonstrar boas práticas de desenvolvimento

## 🛠️ Tecnologias Requeridas

- **Vue.js** (Composition API)
- **Vue Router**
- **Vuex**  (para gerenciamento de estado)
- **Vite** (como bundler)
- **PWA Plugin** (para funcionalidades PWA)
- **CSS/SCSS** (para estilização)

## 📱 Funcionalidades do Sistema

### 1. Tela Inicial (Home)
- **Layout**: Tela principal com dois botões centralizados
- **Funcionalidades**:
  - Botão "Criar Venda" - navega para a tela de produtos
  - Botão "Listar Vendas" - navega para a tela de histórico de vendas
- **Design**: Interface limpa e moderna

### 2. Tela de Produtos e Carrinho
- **Layout**: Duas colunas responsivas
  - **Coluna Esquerda (70%)**: Grid de cards de produtos
  - **Coluna Direita (30%)**: Carrinho de compras
- **Funcionalidades**:
  - **Produtos**:
    - Cards com imagem, nome, preço e botão "Adicionar ao Carrinho"
    - Busca/filtro de produtos
  - **Carrinho**:
    - Lista dos produtos adicionados
    - Quantidade ajustável por produto
    - Subtotal por item
    - Total geral
    - Botão "Finalizar Venda"
- **Estado**: Gerenciar produtos e carrinho no store

### 3. Tela de Conclusão
- **Layout**: Tela de sucesso com informações da venda
- **Funcionalidades**:
  - Mensagem de sucesso
  - Resumo da venda (total, quantidade de itens)
  - Botão "Nova Venda" - volta para tela de produtos
  - Botão "Voltar ao Início" - navega para home
- **Design**: Feedback visual positivo

## 📊 Estrutura de Dados

### Produto
```javascript
{
  id: number,
  name: string,
  price: number,
  image: string,
  description: string,
  category: string
}
```

### Item do Carrinho
```javascript
{
  productId: number,
  quantity: number,
  price: number,
  name: string
}
```

### Venda
```javascript
{
  id: number,
  items: Array<ItemCarrinho>,
  total: number,
  date: Date,
  status: 'completed'
}
```

## 📁 Estrutura de Arquivos Sugerida

```
src/
├── components/
│   ├── ProductCard.vue
│   ├── ShoppingCart.vue
│   ├── CartItem.vue
│   └── Header.vue
├── views/
│   ├── Home.vue
│   ├── Products.vue
│   └── Success.vue
├── store/
│   ├── index.js
│   ├── modules/
│   │   ├── products.js
│   │   ├── cart.js
│   │   └── sales.js
├── router/
│   └── index.js
├── assets/
│   ├── styles/
│   └── images/
└── utils/
    └── helpers.js
```

## 🚀 Critérios de Avaliação

### Funcionalidade 
- ✅ PWA funcionando corretamente
- ✅ Navegação entre telas
- ✅ Gerenciamento de estado
- ✅ Funcionalidades do carrinho
- ✅ Persistência de dados

### Código 
- ✅ Estrutura organizada
- ✅ Componentes reutilizáveis
- ✅ Boas práticas Vue.js
- ✅ Performance otimizada
- ✅ Código limpo e documentado

## 🎯 Bônus (Diferencial)

- Implementar testes unitários
- Adicionar animações CSS/JS
- Implementar modo escuro
- Adicionar notificações push
- Implementar busca avançada
- Adicionar categorias de produtos
- Implementar cupom de desconto
- Adicionar histórico de vendas

## ⏱️ Tempo Estimado

**3-5 dias** para implementação completa

## 🎉 Dicas

- Comece pela estrutura básica e navegação
- Implemente o gerenciamento de estado desde o início
- Teste a responsividade em diferentes dispositivos
- Mantenha o código organizado e componentizado
- Documente suas decisões técnicas
- Teste todas as funcionalidades antes de entregar

---

**Boa sorte! 🚀** 
