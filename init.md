# BlockEstate - Real Estate Platform

## Project Overview

BlockEstate is a modern real estate platform that serves as a digital marketplace for property investment and trading. The platform integrates blockchain technology, AR/VR capabilities, and Web3 features to revolutionize real estate transactions. Users can browse, display, and purchase properties using cryptocurrencies, with NFTs representing property ownership shares.

**Key Features:**

- Property tokenization through NFTs (starting from $10 investments)
- Monthly rental income distribution
- AR/VR property viewing capabilities
- Blockchain-based secure transactions
- Digital wallet integration
- Property marketplace with filtering and search

## Technology Stack

**Frontend:**

- React 18.2.0 with React Router DOM
- CSS3 for styling
- FontAwesome icons
- Responsive design for mobile and desktop

**Backend:**

- Node.js with Express.js
- MongoDB with Mongoose ODM
- JWT authentication
- Cloudinary for image storage
- Multiple payment gateways (Stripe, Paytm)
- Email services (SendGrid, SMTP)

**Key Dependencies:**

- `bcryptjs` - Password hashing
- `jsonwebtoken` - JWT authentication
- `mongoose` - MongoDB object modeling
- `cloudinary` - Image upload and management
- `express-fileupload` - File upload handling
- `cors` - Cross-origin resource sharing
- `validator` - Input validation

## Project Structure

```
src/
├── components/          # React components
│   ├── misc/           # Miscellaneous components (Header, Property, QnA, etc.)
│   ├── navigations/    # Navigation components (Footer, MenuBar)
│   └── pages/          # Page components (Home, About, FAQ, MarketPlace, etc.)
├── backend/            # Node.js backend
│   ├── controllers/    # Route controllers
│   ├── middlewares/    # Custom middleware
│   ├── models/         # MongoDB schemas
│   ├── routes/         # API routes
│   └── utils/          # Utility functions
├── datas/              # Static data (properties, FAQs)
├── images/             # Static images and assets
└── layout/             # Layout components
```

## Building and Running

### Prerequisites

- Node.js (v14 or higher)
- MongoDB database
- Cloudinary account for image storage
- Environment variables configuration

### Installation

```bash
npm install
```

### Environment Setup

Copy `src/backend/config/config.env.example` to create your `.env` file with:

- MongoDB connection string
- JWT secrets
- Cloudinary credentials
- Payment gateway keys
- Email service credentials

### Development Mode

```bash
npm start
```

This runs both frontend and backend concurrently:

- Frontend: React development server
- Backend: Node.js server on port 3099 (default)

### Production Build

```bash
npm run build
```

### Testing

```bash
npm test
```

## Development Conventions

**Code Style:**

- ES6+ JavaScript syntax
- React functional components with hooks
- Modular CSS files for component styling
- Consistent indentation and formatting

**API Structure:**

- RESTful API design
- Base route: `/api/v1/`
- Resource-based routing (users, products, orders, payments)
- JWT-based authentication

**Database Conventions:**

- Mongoose schemas with timestamps
- Referential relationships between collections
- Soft delete patterns using date fields
- Slug generation for SEO-friendly URLs

**Security Practices:**

- Input validation using `validator` library
- Password hashing with `bcryptjs`
- JWT token authentication
- CORS configuration
- File upload restrictions

## Key Models

**Product (Property):**

- Property details, pricing, images
- Category and brand relationships
- Verification and feature status
- Geographic district availability

**User:**

- Authentication and profile management
- Cart and wishlist functionality
- Rating and review capabilities

**Order & Payment:**

- Transaction processing
- Payment gateway integration
- Order status tracking

## Features in Development

The platform includes placeholder features for:

- AR/VR property viewing (mobile-ready UI components)
- Blockchain integration (wallet connection UI)
- NFT property tokenization
- Multi-payment gateway support

## Notes

- Database connection is currently commented out in `server.js`
- The project uses both MongoDB and SQLite3 (for different purposes)
- Image compression and watermarking utilities are available
- Email notification system is implemented
- Real-time features may use Socket.io (model exists)
