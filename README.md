# SIC ( Sistema integrado de cardapio) D` Jesus — Sistema de Gestão

Sistema completo de cardápio online e gerenciamento de pedidos para lojistas em geral

## Funcionalidades

- **Cardápio público** com categorias, promoções e carrinho de compras
- **Sistema de pedidos** com cálculo automático de taxas por bairro, cartão e cupons
- **Painel administrativo** para acompanhamento de pedidos em tempo real
- **PDV (Balcão)** para lançamento de pedidos presenciais
- **Controle de Caixa** com fechamento diário
- **Gestão de Entregadores** com mapa em tempo real
- **Painel da Loja** para cadastro de produtos e horários
- **Relatórios** com gráficos de faturamento
- **Rastreamento** em tempo real via WebSocket + Mapbox
- **Notificações WhatsApp** automáticas via Evolution API

## Tecnologias

| Camada | Tecnologia |
|--------|-----------|
| Frontend | HTML5, CSS3, JavaScript (vanilla) |
| Banco de Dados | Firebase Firestore |
| Backend | Node.js + Express |
| Mapas | Mapbox GL JS, GraphHopper |
| Auth | bcryptjs + localStorage |
| Tempo Real | WebSocket externo |

## Estrutura

```
/
├── index.html           — Cardápio público
├── admin.html           — Painel de pedidos
├── balcao.html          — PDV / Balcão
├── caixa.html           — Controle de caixa
├── dashboard.html       — Dashboard com menu lateral
├── entregador.html      — Gestão de entregas
├── login.html           — Login administrativo
├── painelLoja.html      — Cadastro de produtos/horários
├── relatorios.html      — Relatórios
├── superadmin.html      — Admin de usuários
├── alterar-senha.html   — Troca de senha
├── view/cart.html       — Carrinho de compras
├── js/                  — Scripts do frontend
├── css/                 — Folhas de estilo
├── backend/             — API Node.js (Express)
└── img/                 — Imagens
```

## Setup

```bash
git clone <repo>
cd backend
cp .env .env.local     # ajustar variáveis
npm install
npm start
```

Abra `index.html` no navegador para o cardápio público, ou `login.html` para o painel admin.

## Licença

Uso interno — Fábrica de Salgados Costa
