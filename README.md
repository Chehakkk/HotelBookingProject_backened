# Hospitality - Hotel Booking Platform

A Django-based hotel booking system similar to MakeMyTrip, providing comprehensive hospitality services including hotel search, booking management, payment processing, and user account management.

## 🏨 Features

- **Hotel Search & Discovery**: Advanced search with location, price, amenities, and ratings filters
- **Real-time Booking**: Instant reservations with availability checking
- **Payment Processing**: Secure payment gateway integration with multiple options
- **User Management**: Customer accounts, profiles, and booking history
- **Policy Management**: Cancellation, refund, and booking policies
- **Dynamic Pricing**: Seasonal rates, discounts, and demand-based pricing

## 📁 Project Structure

```
hospitality/
├── hotels/                      # Hotel listings, rooms, amenities, reviews
├── booking/                     # Reservation management and tracking
├── search/                      # Advanced search and filtering
├── pricing_payments/            # Pricing engine and payment processing
├── policies/                    # Terms, cancellation, and refund policies
├── account/                     # User authentication and profiles
├── static/                      # CSS, JS, images
├── templates/                   # HTML templates
└── manage.py
```

## 🛠️ Technology Stack

- **Backend**: Django 4.x, Python 3.x
- **Database**: PostgreSQL/MySQL/SQLite
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap
- **Payments**: Stripe/Razorpay integration
- **Authentication**: Django Auth system

## ⚙️ Quick Setup

1. **Clone and setup environment**
   ```bash
   git clone <repository-url>
   cd hospitality
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

2. **Configure environment**
   Create `.env` file:
   ```env
   SECRET_KEY=your_secret_key
   DEBUG=True
   DATABASE_URL=your_database_url
   STRIPE_PUBLIC_KEY=your_stripe_public_key
   STRIPE_SECRET_KEY=your_stripe_secret_key
   EMAIL_HOST_USER=your_email
   EMAIL_HOST_PASSWORD=your_password
   ```

3. **Database setup**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   python manage.py createsuperuser
   python manage.py runserver
   ```

Visit `http://127.0.0.1:8000` to access the application.

## 🏗️ App Architecture

### Hotels App
- Hotel listings, room types, amenities
- Image galleries and location data
- Ratings, reviews, and availability calendar

### Booking App
- Reservation creation and management
- Check-in/out date handling
- Booking status tracking and modifications

### Search App
- Advanced filtering by location, price, amenities
- Map integration and sorting options
- Search suggestions and recent searches

### Pricing & Payments App
- Dynamic pricing engine with seasonal rates
- Payment gateway integration
- Transaction processing and invoice generation

### Policies App
- Cancellation and refund policies
- Terms and conditions management
- Booking rules and restrictions

### Account App
- User registration and authentication
- Profile management and booking history
- Password reset and email verification

## 📊 Usage

**For Customers:**
- Search hotels by location, dates, and preferences
- View hotel details, amenities, and reviews
- Make bookings with secure payment processing
- Manage account and view booking history

**For Administrators:**
- Manage hotel information and room inventory
- Monitor bookings and reservations
- Control pricing and promotional offers
- Update policies and terms

## 🔒 Security Features

- CSRF and XSS protection
- Secure payment processing
- User authentication and authorization
- Input validation and password encryption

## 🚀 Deployment

**Production Setup:**
- Set `DEBUG = False`
- Configure production database
- Set up SSL certificates
- Configure static file serving
- Set up email backend

**Deployment Options:**
- Heroku, AWS EC2, DigitalOcean
- Docker containerization support

## 🧪 Testing

```bash
python manage.py test                    # Run all tests
python manage.py test hotels            # Test specific app
```

## 📈 Key Features Implementation

- **Search Engine**: Location-based search with advanced filters
- **Booking System**: Real-time availability and instant confirmation
- **Payment Gateway**: Multiple payment options with secure processing
- **User Dashboard**: Comprehensive booking management interface
- **Admin Panel**: Hotel and reservation management tools
- **Review System**: Customer feedback and rating functionality

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/NewFeature`)
3. Commit changes (`git commit -m 'Add NewFeature'`)
4. Push to branch (`git push origin feature/NewFeature`)
5. Create Pull Request


