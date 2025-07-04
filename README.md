# STREETFLOW - Premium Streetwear E-commerce Platform

A modern, dark-themed e-commerce platform built with React and Express.js, specializing in streetwear fashion. Features a sleek urban design with full shopping cart functionality, wishlist management, and responsive mobile experience.

## ✨ Features

### Frontend
- **Modern Dark Theme** - Sleek black interface with cyan accent colors
- **Responsive Design** - Optimized for mobile, tablet, and desktop
- **Product Catalog** - Browse by category with filtering and search
- **Shopping Cart** - Add, remove, and manage quantities
- **Wishlist** - Save favorite products for later
- **Product Details** - Full product pages with size/color selection
- **Mobile Navigation** - Bottom navigation bar for mobile users
- **Real-time Updates** - Cart count and wishlist sync across components

### Backend
- **RESTful API** - Express.js with TypeScript
- **Session Management** - Guest checkout without registration
- **Data Validation** - Zod schemas for request validation
- **In-memory Storage** - Fast development with interface for database integration
- **CORS Support** - Configured for frontend integration

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks and context
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Accessible component primitives
- **TanStack Query** - Server state management
- **Wouter** - Lightweight client-side routing
- **Vite** - Fast development and building

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **TypeScript** - Type-safe server development
- **Drizzle ORM** - Type-safe SQL query builder
- **Zod** - Schema validation
- **tsx** - TypeScript execution

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd streetflow-ecommerce
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   ```
   http://localhost:5000
   ```

## 📁 Project Structure

```
streetflow-ecommerce/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   │   ├── ui/        # shadcn/ui components
│   │   │   ├── Header.tsx
│   │   │   ├── ProductCard.tsx
│   │   │   ├── Cart.tsx
│   │   │   └── MobileNav.tsx
│   │   ├── context/       # React context providers
│   │   │   └── CartContext.tsx
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utilities and configurations
│   │   ├── pages/         # Route components
│   │   │   ├── Home.tsx
│   │   │   ├── ProductDetail.tsx
│   │   │   └── Cart.tsx
│   │   ├── App.tsx        # Main application component
│   │   ├── main.tsx       # Entry point
│   │   └── index.css      # Global styles and theme
│   └── index.html         # HTML template
├── server/                # Backend Express application
│   ├── index.ts          # Server entry point
│   ├── routes.ts         # API route definitions
│   ├── storage.ts        # Data storage implementation
│   └── vite.ts           # Vite integration
├── shared/               # Shared TypeScript definitions
│   └── schema.ts         # Database schema and types
├── package.json          # Dependencies and scripts
├── vite.config.ts        # Vite configuration
├── tailwind.config.ts    # Tailwind CSS configuration
└── tsconfig.json         # TypeScript configuration
```

## 🎨 Design System

### Color Palette
- **Background**: Pure black (`#000000`)
- **Secondary**: Dark gray (`#1a1a1a`)
- **Accent**: Cyan (`#00bcd4`)
- **Text**: White (`#ffffff`)
- **Muted**: Light gray (`#cccccc`)

### Typography
- **Headings**: Bold, modern sans-serif
- **Body**: Clean, readable font stack
- **Sizes**: Responsive scaling for mobile/desktop

### Components
- **Cards**: Rounded corners with subtle shadows
- **Buttons**: Solid accent color with hover effects
- **Forms**: Dark inputs with cyan focus states
- **Navigation**: Clean, minimal design

## 🛒 E-commerce Features

### Product Management
- Product catalog with 8 sample items
- Categories: Hoodies, T-Shirts, Sneakers, Accessories
- Product ratings and review counts
- Multiple product images
- Size and color variants
- Sale pricing with original price display

### Shopping Cart
- Add products with size/color selection
- Quantity management (increase/decrease)
- Remove individual items
- Clear entire cart
- Real-time price calculations
- Persistent cart across sessions

### Wishlist
- Heart icon toggle on product cards
- Add/remove from wishlist
- Visual feedback for wishlist status
- Persistent across sessions

## 📱 Mobile Experience

### Responsive Design
- Mobile-first approach
- Breakpoints for tablet and desktop
- Touch-friendly interface elements
- Optimized image sizes

### Mobile Navigation
- Bottom navigation bar
- Quick access to Home, Search, Wishlist, Cart, Profile
- Cart badge with item count
- Smooth transitions

### Mobile Optimizations
- Larger touch targets
- Simplified navigation
- Optimized image loading
- Fast scroll performance

## 🔧 API Endpoints

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product by ID
- `GET /api/products?category=:category` - Filter by category
- `GET /api/products?search=:query` - Search products

### Cart
- `GET /api/cart` - Get cart items
- `POST /api/cart` - Add item to cart
- `PUT /api/cart/:id` - Update cart item quantity
- `DELETE /api/cart/:id` - Remove cart item
- `DELETE /api/cart` - Clear cart

### Wishlist
- `GET /api/wishlist` - Get wishlist items
- `POST /api/wishlist` - Add to wishlist
- `DELETE /api/wishlist/:productId` - Remove from wishlist
- `GET /api/wishlist/:productId` - Check if in wishlist

## 🚀 Build and Deployment

### Development
```bash
npm run dev          # Start development server
```

### Production Build
```bash
npm run build        # Build for production
npm start           # Start production server
```

### Build Outputs
- `dist/public/` - Frontend static files
- `dist/server.js` - Backend server bundle

## 🧪 Development Commands

```bash
# Start development server
npm run dev

# Build client only
npm run build:client

# Build server only  
npm run build:server

# Full production build
npm run build

# Start production server
npm start
```

## 🎯 Key Features Explained

### Session Management
- Automatic session ID generation for guest users
- No registration required for shopping
- Persistent cart and wishlist across browser sessions

### State Management
- React Context for cart state
- TanStack Query for server state caching
- Optimistic updates for better UX
- Cache invalidation on mutations

### Component Architecture
- Reusable UI components with shadcn/ui
- Custom components for e-commerce functionality
- Type-safe props with TypeScript interfaces
- Responsive design with Tailwind CSS

### Performance Optimizations
- Image lazy loading
- Query caching with React Query
- Efficient re-renders with React.memo
- Optimized bundle size with Vite

## 🔮 Future Enhancements

### Planned Features
- User authentication and accounts
- Payment processing integration
- Order history and tracking
- Product reviews and ratings
- Advanced search and filtering
- Inventory management
- Admin dashboard
- Email notifications

### Technical Improvements
- Database integration (PostgreSQL)
- Image optimization and CDN
- SEO optimization
- Progressive Web App (PWA)
- Testing suite (Jest, Cypress)
- CI/CD pipeline
- Error monitoring

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- **Radix UI** for accessible component primitives
- **Tailwind CSS** for utility-first styling
- **Unsplash** for high-quality product images
- **Lucide React** for beautiful icons
- **TanStack Query** for excellent data fetching

---

**STREETFLOW** - Where street meets flow. Premium streetwear for the modern urban lifestyle.
