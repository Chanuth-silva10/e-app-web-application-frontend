# E-Commerce Web Application - Frontend

A modern, responsive e-commerce web application built with React.js, featuring a complete shopping experience with user authentication, product management, and administrative capabilities.

## 🚀 Features

### Customer Features
- **User Authentication**: Sign up, login, logout, and forgot password functionality
- **Product Browsing**: Browse products by categories with advanced filtering and sorting
- **Product Search**: Search products with real-time results
- **Product Details**: Detailed product view with image zoom functionality
- **Shopping Cart**: Add/remove items, quantity management, and cart persistence
- **Responsive Design**: Mobile-friendly interface with Tailwind CSS
- **Product Categories**: Browse by categories (Mobiles, Cameras, Watches, Airpods, etc.)

### Admin Features
- **Admin Panel**: Dedicated admin interface for management
- **Product Management**: Add, edit, and delete products
- **User Management**: View and manage user accounts
- **Role-based Access**: Admin and General user roles
- **Image Upload**: Cloudinary integration for product images
- **Product Analytics**: View all products and user data

### Technical Features
- **State Management**: Redux Toolkit for global state management
- **Routing**: React Router v6 for navigation
- **API Integration**: RESTful API communication
- **Toast Notifications**: User feedback with react-toastify
- **Loading States**: Skeleton loading animations
- **Image Optimization**: Base64 conversion and cloud storage

## 🛠️ Tech Stack

- **Frontend Framework**: React 18.2.0
- **State Management**: Redux Toolkit 2.2.1
- **Routing**: React Router DOM 6.22.1
- **Styling**: Tailwind CSS 3.4.1
- **UI Components**: React Icons 5.0.1
- **Notifications**: React Toastify 10.0.4
- **Date Handling**: Moment.js 2.30.1
- **Build Tool**: Create React App 5.0.1

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── Header.js       # Navigation header with search
│   ├── Footer.js       # Footer component
│   ├── CategoryList.js # Product category display
│   ├── BannerProduct.js # Hero banner
│   ├── VerticalCard.js # Product card layout
│   ├── HorizontalCardProduct.js # Horizontal product cards
│   ├── UploadProduct.js # Product upload form
│   ├── AdminProductCard.js # Admin product management
│   └── ...
├── pages/              # Main application pages
│   ├── Home.js         # Homepage with product showcase
│   ├── Login.js        # User authentication
│   ├── SignUp.js       # User registration
│   ├── ProductDetails.js # Individual product view
│   ├── Cart.js         # Shopping cart
│   ├── AdminPanel.js   # Admin dashboard
│   ├── AllProducts.js  # Product management
│   ├── CategoryProduct.js # Category-wise products
│   └── ...
├── helpers/            # Utility functions
│   ├── displayCurrency.js # Currency formatting
│   ├── addToCart.js    # Cart functionality
│   ├── uploadImage.js  # Image upload utilities
│   ├── productCategory.js # Product categories
│   └── ...
├── store/              # Redux store configuration
│   ├── store.js        # Store setup
│   └── userSlice.js    # User state management
├── context/            # React context
├── common/             # API configurations and constants
└── assets/             # Static assets
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Backend API server running on `http://localhost:8080`

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd e-app-web-application-frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   - Ensure your backend API is running on `http://localhost:8080`
   - Update API endpoints in `src/common/index.js` if needed

4. **Start the development server**
   ```bash
   npm start
   ```

5. **Open your browser**
   - Navigate to `http://localhost:3000`

### Available Scripts

- `npm start` - Runs the app in development mode
- `npm test` - Launches the test runner
- `npm run build` - Builds the app for production
- `npm run eject` - Ejects from Create React App (one-way operation)

## 🔧 Configuration

### API Configuration

The application communicates with a backend API. Update the backend domain in `src/common/index.js`:

```javascript
const backendDomin = "http://localhost:8080"
```

### Tailwind CSS

Tailwind configuration is available in `tailwind.config.js`. Customize the design system as needed.

## 📱 Responsive Design

The application is fully responsive and optimized for:
- Desktop (1024px+)
- Tablet (768px - 1023px)
- Mobile (320px - 767px)

## 🔐 User Roles

### General User
- Browse and search products
- Add products to cart
- View product details
- Manage personal cart

### Admin User
- All general user capabilities
- Access to admin panel
- Product management (CRUD operations)
- User management
- View analytics and reports

## 🛒 Product Categories

The application supports the following product categories:
- Airpods
- Cameras
- Earphones
- Mobiles
- Mouse
- Printers
- Processors
- Refrigerators
- Speakers
- Trimmers
- Televisions
- Watches

## 🎨 UI Components

### Reusable Components
- **ProductCard**: Display product information
- **CategoryList**: Category navigation
- **SearchBar**: Product search functionality
- **LoadingSpinner**: Loading state indicators
- **Toast Notifications**: User feedback messages

### Layout Components
- **Header**: Navigation with search and cart
- **Footer**: Site information and links
- **Sidebar**: Category filters and navigation

## 🔄 State Management

The application uses Redux Toolkit for state management:

- **User Slice**: Authentication and user data
- **Cart State**: Shopping cart management
- **Product State**: Product data and filters

## 📡 API Integration

### Authentication Endpoints
- POST `/api/signup` - User registration
- POST `/api/signin` - User login
- GET `/api/user-details` - Get current user
- GET `/api/userLogout` - User logout

### Product Endpoints
- GET `/api/get-product` - Get all products
- POST `/api/upload-product` - Add new product
- POST `/api/update-product` - Update product
- POST `/api/product-details` - Get product details
- POST `/api/category-product` - Get category products

### Cart Endpoints
- POST `/api/addtocart` - Add to cart
- GET `/api/countAddToCartProduct` - Get cart count
- GET `/api/view-card-product` - Get cart items
- POST `/api/update-cart-product` - Update cart item
- POST `/api/delete-cart-product` - Remove from cart

## 🚀 Deployment

### Production Build

1. **Create production build**
   ```bash
   npm run build
   ```

2. **Deploy to hosting service**
   - The `build` folder contains the production-ready application
   - Deploy to services like Netlify, Vercel, or AWS S3

### Environment Variables

For production deployment, consider setting up environment variables for:
- API base URL
- Image upload service keys
- Analytics tracking IDs

## 🙏 Acknowledgments

- Create React App for the initial setup
- Tailwind CSS for the utility-first CSS framework
- React Icons for the comprehensive icon library
- Redux Toolkit for efficient state management

## 📞 Support

For support and questions:
- Create an issue in the repository
- Check the documentation
- Review existing issues and discussions

---

**Note**: This frontend application requires a corresponding backend API to function properly. Ensure your backend server is running and accessible before starting the development server.
