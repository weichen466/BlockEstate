# BlockEstate 🏢

A revolutionary digital real estate trading platform that integrates blockchain, AR/VR, and Web3 technologies to make real estate investment simpler, more transparent, and accessible.

## 🌟 Project Features

BlockEstate is a modern real estate platform that lowers the barrier to real estate investment to just $10 through NFT tokenization, while providing:

- **NFT Real Estate Tokenization** - Fractionalize properties into NFT shares starting from $10
- **Monthly Rental Income** - Automatic monthly rental income distribution to digital wallets
- **AR/VR Property Viewing** - Immersive property browsing experience
- **Blockchain Transactions** - Secure and transparent real estate transactions and ownership verification
- **Instant Liquidity** - Buy and sell NFT property shares anytime
- **Zero Hidden Fees** - No entry fees, exit fees, or capital gains taxes

## 🚀 Technology Stack

### Frontend Technologies
- **React 18.2.0** - Modern user interface
- **React Router DOM** - Single page application routing
- **CSS3** - Responsive styling
- **FontAwesome** - Icon system

### Backend Technologies
- **Node.js + Express.js** - High-performance server
- **MongoDB + Mongoose** - Flexible data storage
- **JWT Authentication** - Secure user authentication
- **Cloudinary** - Cloud image storage and management
- **Multiple Payment Gateways** - Stripe, Paytm integration
- **SendGrid/SMTP** - Email notification system

### Blockchain Integration
- **Web3 Wallet Connection** - Support for MetaMask and other mainstream wallets
- **NFT Smart Contracts** - Real estate tokenization
- **Blockchain Payments** - Cryptocurrency transaction support

## 📦 Quick Start

### Requirements
- Node.js (v14 or higher)
- MongoDB database
- Cloudinary account
- Modern browser (Web3 support)

### Installation Steps

1. **Clone the project**
```bash
git clone https://github.com/weichen466/CryptoEstate.git
cd CryptoEstate
```

2. **Install dependencies**
```bash
npm install
```

3. **Environment Configuration**
Copy the configuration file and fill in your credentials:
```bash
cp src/backend/config/config.env.example src/backend/config/config.env
```

Edit the `config.env` file and add the following configuration:
```env
# Database
MONGO_URI=your_mongodb_connection_string

# JWT Secret
JWT_SECRET=your_jwt_secret_key

# Cloudinary
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Payment Gateways (Optional)
STRIPE_API_KEY=your_stripe_key
PAYTM_MID=your_paytm_mid

# Email Service
SENDGRID_API_KEY=your_sendgrid_key
```

4. **Start Development Server**
```bash
npm start
```

The application will run at:
- Frontend: http://localhost:3000
- Backend: http://localhost:3099

## 🏗️ Project Structure

```
CryptoEstate/
├── public/                    # Static resources
├── src/
│   ├── components/           # React components
│   │   ├── misc/            # Common components (Header, Property, QnA, etc.)
│   │   ├── navigations/     # Navigation components
│   │   └── pages/           # Page components
│   ├── backend/             # Node.js backend
│   │   ├── controllers/     # Controllers
│   │   ├── middlewares/     # Middleware
│   │   ├── models/          # Data models
│   │   ├── routes/          # API routes
│   │   └── utils/           # Utility functions
│   ├── datas/               # Static data
│   ├── images/              # Image resources
│   └── layout/              # Layout components
├── package.json
└── README.md
```

## 🔧 Core Features

### Real Estate Marketplace
- Browse investable property projects
- View detailed property information and images
- Filter properties by region, price, type
- AR/VR virtual property viewing experience

### Investment Management
- Purchase property NFT shares (minimum $10)
- View investment portfolio and returns
- Receive monthly rental dividends automatically
- Sell NFT shares anytime

### User System
- Registration and authentication
- Digital wallet connection
- Personal profile management
- Transaction history

### Payment System
- Multiple payment method support
- Cryptocurrency payments
- Fiat payment gateways
- Secure transaction processing

## 🛡️ Security Features

- **JWT Authentication** - Secure user session management
- **Password Encryption** - bcryptjs hashing algorithm
- **Input Validation** - Comprehensive data validation
- **CORS Protection** - Cross-origin request security
- **File Upload Security** - Strict file type checking

## 🚦 Available Scripts

```bash
# Development mode (frontend and backend run simultaneously)
npm start

# Build production version
npm run build

# Run tests
npm test

# Eject Create React App configuration
npm run eject
```

## 🌐 API Documentation

The backend API is based on RESTful design, main endpoints include:

- **User Management**: `/api/v1/users`
- **Property Management**: `/api/v1/products`
- **Order Management**: `/api/v1/orders`
- **Payment Processing**: `/api/v1/payments`

For detailed API documentation, please refer to the route definitions in the backend code.

## 🧪 Testing

The project includes a complete test suite:
```bash
# Run all tests
npm test

# Run specific test file
npm test -- --testPathPattern=App.test.js
```

## 📱 Responsive Design

BlockEstate adopts a mobile-first responsive design, supporting:
- Desktop (1200px+)
- Tablet (768px-1199px)
- Mobile (320px-767px)

## 🔮 Future Roadmap

- [ ] Complete AR/VR property viewing functionality
- [ ] More blockchain network support
- [ ] AI-driven property recommendations
- [ ] Community governance features
- [ ] Mobile app development
- [ ] Multi-language support

## 🤝 Contributing Guidelines

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Create a Pull Request

## 👥 Team

BlockEstate is built by a passionate development team dedicated to changing the real estate investment industry through technological innovation.

---

**Making real estate investment simple, transparent, and accessible - BlockEstate**