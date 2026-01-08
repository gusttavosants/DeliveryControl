# 🚚 Delivery Dispatch Hero

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white)](https://nestjs.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)](https://vercel.com/)

A comprehensive delivery management system designed to streamline order dispatch, driver assignment, and delivery tracking. Built with a modern full-stack architecture featuring a NestJS backend and React frontend.

## ✨ Features

- 📦 **Order Management**: Create, track, and manage delivery orders with detailed information
- 🚴‍♂️ **Driver Assignment**: Efficiently assign orders to available delivery drivers (motoboys)
- 📍 **Real-time Tracking**: Monitor driver locations and delivery status
- 🗺️ **Route Optimization**: Optimize delivery routes for better efficiency
- 📊 **Statistics & Reports**: Generate insights on delivery performance and trends
- 🔐 **User Authentication**: Secure login system with JWT authentication
- ⚙️ **Advanced Settings**: Configure fees, integrations, user roles, and SLA monitoring
- 📄 **PDF Generation**: Generate reports and delivery documents
- 📦 **Order Batching**: Group orders for bulk processing
- 💰 **Vales Module**: Manage delivery vouchers and allowances

## 🛠️ Tech Stack

| Component | Technology | Description |
|-----------|------------|-------------|
| **Backend** | NestJS (Node.js) | Progressive Node.js framework |
| **Frontend** | React 18 | Modern UI library |
| **Language** | TypeScript | Typed JavaScript |
| **Database** | SQLite | Lightweight database |
| **Build Tool** | Vite | Fast frontend build tool |
| **Styling** | Tailwind CSS | Utility-first CSS framework |
| **UI Components** | shadcn/ui | Beautiful UI components |
| **Package Manager** | Bun | Fast JavaScript runtime |
| **Authentication** | JWT | JSON Web Tokens |
| **Testing** | Jest | Testing framework |
| **Deployment** | Vercel | Cloud platform |

## 📋 Prerequisites

- 🟢 Node.js (v16 or higher)
- 📦 npm or bun
- 🗄️ SQLite (included, no separate installation needed)

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/delivery-dispatch-hero.git
   cd delivery-dispatch-hero
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd ../frontend
   bun install
   ```

## ▶️ Running the Application

### Backend
```bash
cd backend
npm run start:dev
```
> 💡 The backend will run on `http://localhost:3000`

### Frontend
```bash
cd frontend
bun dev
```
> 💡 The frontend will run on `http://localhost:5173`

## 🔗 API Endpoints

### 🔐 Authentication
- `POST /auth/login` - User login

### 🚴‍♂️ Motoboys (Drivers)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/motoboy` | Get all drivers |
| POST | `/motoboy` | Create new driver |
| PUT | `/motoboy/:id` | Update driver |
| DELETE | `/motoboy/:id` | Delete driver |

### 📦 Pedidos (Orders)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/pedido` | Get all orders |
| POST | `/pedido` | Create new order |
| PUT | `/pedido/:id` | Update order |
| DELETE | `/pedido/:id` | Delete order |

### 📊 Statistics
- `GET /statistics` - Get delivery statistics

## 📁 Project Structure

```
delivery-dispatch-hero/
├── backend/
│   ├── src/
│   │   ├── auth/          # 🔐 Authentication module
│   │   ├── motoboy/       # 🚴‍♂️ Driver management
│   │   ├── pedido/        # 📦 Order management
│   │   └── statistics/    # 📊 Statistics and reports
│   ├── test/              # 🧪 End-to-end tests
│   └── database.sqlite    # 🗄️ SQLite database
├── frontend/
│   ├── src/
│   │   ├── components/    # 🧩 Reusable UI components
│   │   ├── pages/         # 📄 Application pages
│   │   ├── hooks/         # 🪝 Custom React hooks
│   │   └── lib/           # 🛠️ Utilities and API functions
│   └── public/            # 📁 Static assets
├── package.json           # 📦 Root package configuration
├── vercel.json            # ☁️ Vercel deployment config
└── README.md              # 📖 This file
```

## 🧪 Testing

### Backend Tests
```bash
cd backend
npm run test          # Unit tests
npm run test:e2e      # End-to-end tests
npm run test:cov      # Test coverage
```

## ☁️ Deployment

The project is configured for deployment on Vercel:

1. Connect your GitHub repository to Vercel
2. Configure the build settings:
   - **Frontend**: Root directory `frontend`, build command `bun run build`
   - **Backend**: Root directory `backend`, build command `npm run build`
3. Deploy automatically on push or manually trigger deployment

## 🤝 Contributing

1. Fork the repository 🍴
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -am 'Add new feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Submit a pull request 📝

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support, please open an issue in the GitHub repository or contact the development team.
