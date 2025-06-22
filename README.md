# New-beauty-csm
# Beauty CMS 🏪

A comprehensive salon management system designed specifically for beauty professionals, featuring product search with affiliate integration, appointment management, and client relationship tools.

## ✨ Features

### 🛍️ Product Search & Affiliate Integration
- **Amazon Product Search**: Browse millions of beauty products
- **Affiliate Commission Tracking**: Earn commissions on product sales
- **Category Filtering**: Hair care, nail products, tools, equipment
- **Professional Recommendations**: Curated product suggestions

### 📅 Appointment Management
- **Smart Booking System**: Prevent double-booking with real-time availability
- **Deposit Management**: Secure Stripe integration for deposits
- **Status Tracking**: Booked, confirmed, completed, cancelled, no-show
- **Recurring Appointments**: Automated scheduling for regular clients

### �� Payment Processing
- **Stripe Integration**: Secure payment processing
- **Deposit System**: £10 deposit requirement with automated reminders
- **Multiple Payment Methods**: Card, cash, loyalty points redemption
- **Refund Management**: Automated refund processing

### �� Client Management
- **Comprehensive Profiles**: Hair type, allergies, preferences, loyalty points
- **Client History**: Complete appointment and payment history
- **Product Usage Tracking**: What products were used in each appointment
- **Analytics**: Most frequent services, average spend, visit patterns

### �� Specialized Beauty Features
- **Hair & Nail Profiles**: Detailed client preferences and requirements
- **Allergy Tracking**: Important safety information
- **Loyalty Points System**: Reward repeat clients
- **Client Notes**: Detailed appointment and preference notes

## 🚀 Tech Stack

- **Backend**: FastAPI (Python)
- **Database**: SQLite with SQLAlchemy ORM
- **Payment**: Stripe API
- **Product Search**: Amazon Product Advertising API
- **Authentication**: JWT tokens
- **Email**: SMTP integration
- **Background Tasks**: Async notification system

## �� API Endpoints

### Core Features
- `GET /api/v1/clients/` - Client management
- `GET /api/v1/appointments/` - Appointment booking
- `GET /api/v1/services/` - Service catalog
- `GET /api/v1/products/search` - Product search (Amazon)
- `GET /api/v1/analytics/` - Business analytics

### Advanced Features
- `GET /api/v1/clients/{id}/history` - Client history with analytics
- `GET /api/v1/clients/{id}/profile` - Detailed client profiles
- `GET /api/v1/usage-analytics/` - Product usage analytics
- `GET /api/v1/reorder-suggestions/` - Inventory management

## ��️ Installation

```bash
# Clone the repository
git clone https://github.com/JakeS-dev/beauty-cms.git
cd beauty-cms

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your API keys

# Run database migrations
alembic upgrade head

# Start the server
uvicorn main:app --reload
```

## 🔧 Configuration

Required environment variables:
```env
# Stripe Configuration
STRIPE_SECRET_KEY=sk_test_...
STRIPE_WEBHOOK_SECRET=whsec_...

# Amazon Product Advertising API
AMAZON_ACCESS_KEY_ID=your_access_key
AMAZON_SECRET_ACCESS_KEY=your_secret_key
AMAZON_ASSOCIATE_TAG=your_associate_tag

# Email Configuration
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USERNAME=your_email@gmail.com
SMTP_PASSWORD=your_app_password
```

## 📈 Business Benefits

### For Salon Owners
- **Increased Revenue**: Affiliate commissions on product sales
- **Better Client Retention**: Loyalty points and detailed profiles
- **Efficient Operations**: Automated booking and payment processing
- **Data Insights**: Analytics on services, products, and client behavior

### For Beauticians
- **Easy Product Discovery**: Search and purchase professional products
- **Client Management**: Comprehensive client profiles and history
- **Streamlined Booking**: Simple appointment scheduling
- **Professional Tools**: Everything needed to run a successful salon

## 🔮 Roadmap

- [ ] **Mobile App**: React Native client app
- [ ] **Multi-location Support**: Chain salon management
- [ ] **Advanced Analytics**: Predictive insights and trends
- [ ] **Inventory Management**: Stock tracking and reorder automation
- [ ] **Marketing Tools**: Email campaigns and promotions
- [ ] **Integration APIs**: Connect with other salon software

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support, email support@beautycms.com or create an issue in this repository.

---

**Built with ❤️ for the beauty industry**
