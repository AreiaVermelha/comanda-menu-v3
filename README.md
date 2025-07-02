# 🍽️ Comanda Menu - Frontend

Aplicação **React** desenvolvida para gerenciar comandas e pedidos em bares e restaurantes de pequeno porte. Esta interface se comunica com uma API Express para autenticação, controle de produtos, pedidos e notificações em tempo real.

---

## ⚙️ Tecnologias Utilizadas

- **React 18**
- **React Router DOM v6**
- **Tailwind CSS** (estilização)
- **Axios** (requisições HTTP)
- **Socket.io Client** (comunicação em tempo real)
- **Firebase Cloud Messaging** (notificações push)
- **React Hot Toast** (feedback de ações)
- **HTML2Canvas** (captura de tela para impressão ou download)

## 👷‍♂️ Configuração do Ambiente
1. Clone este repositório:
```bash
git clone https://github.com/JackSSads/comanda-menu-v3
```

2. Navegue até o diretório do projeto:
```bash
cd comanda-menu-v3
```

3. Instale as dependências:
```bash
npm install
```

4. Crie um arquivo `.env` 
```bash
REACT_APP_BASE_URL_BACK=http://localhost:3001
REACT_APP_BASE_URL_FRONT=http://localhost:3000
REACT_APP_NODE_ENV=development
REACT_APP_VAPID_KEY_PUBLICA=
REACT_APP_FAVICON_URL=
```

5. Inicie o servidor de desenvolvimento:
```bash
npm start
```

## 📁 Estrutura de Pastas
```
src/
├── components/
    ├── calc/index.jsx
    ├── cardCheck/index.jsx
    ├── cardProduct/index.jsx
    ├── cardProductPreparation/index.jsx
    ├── categories/index.jsx
    ├── check/index.jsx
    ├── clnput/index.jsx
    ├── filter/index.jsx
    ├── footer/index.jsx
    ├── listinProductsForCheck/index.jsx
    ├── loader/index.jsx
    ├── loadingItem/index.jsx
    ├── managerUser/index.jsx
    ├── modalProduct/index.jsx
    ├── modalUser/index.jsx
    ├── navbar/index.jsx
    ├── newCheck/index.jsx
    ├── settings/index.jsx
    ├── sidebar/index.jsx
    └── index.js
├── contexts/
    ├── LoaderContext.jsx
    ├── ToggleSidebar.jsx
    ├── ToggleViewNote.jsx
    └── index.js 
├── hooks/
    ├── ConnectionMonitor.js
    ├── Notifications.js
    ├── UseAlert.js
    ├── UseDebounce.js
    ├── UseFCM.js
    ├── UseSocketEvents.js
    ├── UseVerifyIfClientId.js
├── layouts/
    └── index.js 
├── libs/
    └── icons.js 
├── pages/
    ├── admin/index.jsx
    ├── clientMenu/index.jsx
    ├── closeCheck/index.jsx
    ├── closedChecks/index.jsx
    ├── error/
        ├── 404.jsx
        ├── 404.jsx
        └── index.js 
    ├── firstAccess/index.jsx
    ├── home0/index.jsx
    ├── listingChecks/index.jsx
    ├── listingProducts/index.jsx
    ├── login/index.jsx
    ├── manageUser/index.jsx
    ├── onlineOrders/index.jsx
    ├── preparation/
        ├── bartender.jsx
        └── cuisine.jsx
    ├── salesHistory/index.jsx
    ├── showEditProducts/index.jsx
    ├── waiter/index.jsx
    └── index.js
├── routes/index.jsx
├── service/
    ├── axiosConfig/index.js
    ├── cashier/CashierService.js
    ├── category/CategoryService.js
    ├── check/CheckService.js
    ├── login/LoginService.js
    ├── logout/LogoutService.js
    ├── notification/NotificationService.js
    ├── order/OrderService.js
    ├── payment/PaymentService.js
    ├── product/ProductService.js
    ├── setting/SettingService.js
    ├── socket/SocketService.js
    └── user/UserService.js
├── App.jsx
├── firebase.js
├── index.css
└── index.jsx
```

### 🔐 Autenticação
A autenticação é baseada em JWT. Os tokens são gerados no login e devem ser enviados via `Authorization: Bearer <token>` nas rotas protegidas.

### 🧾 Pagamentos
Integração com Mercado Pago para gerar links de pagamento e receber notificações de retorno via webhook.

### 📲 Notificações Push 
Usa o Firebase Cloud Messaging.
Cada usuário pode registrar um `notify_id` para receber alertas personalizados.

### 🧑‍💻 Autor
[Jackson Souza da Silva](https://github.com/JackSSads)

## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

[API do projeto](https://github.com/JackSSads/comanda-api-v3)
