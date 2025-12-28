# Soft Laundry Delivery System - Business Requirements Documentation

## Table of Contents
1. [System Overview](#system-overview)
2. [User Types and Roles](#user-types-and-roles)
3. [Functional Requirements by User Type](#functional-requirements-by-user-type)
4. [System Dashboard (Admin Panel)](#system-dashboard-admin-panel)
5. [Laundromat Dashboard](#laundromat-dashboard)
6. [Customer Mobile Application](#customer-mobile-application)
7. [Driver Mobile Application](#driver-mobile-application)
8. [Vendor Tablet Application](#vendor-tablet-application)
9. [Order Management Workflows](#order-management-workflows)
10. [Customer Support System](#customer-support-system)
11. [System Features Summary](#system-features-summary)

---

## System Overview

**Soft Laundry** is a complete laundry service delivery platform designed to streamline the connection between customers and local laundromats. The system ensures customers receive convenient, reliable laundry services while providing laundromats and delivery drivers with powerful tools to manage their operations effectively.

### Business Value Proposition

**For Customers:**
- Convenient access to nearby laundromats within their neighborhood
- Multiple service options: pickup, delivery, or drop-off
- Real-time order tracking and notifications
- Flexible payment options
- Scheduled subscription services for regular customers

**For Laundromats:**
- Efficient order management and customer relationship tools
- Automated pricing and billing calculations
- Customer subscription management
- Revenue tracking and analytics
- Streamlined communication with drivers and customers

**For Drivers:**
- Easy order acceptance and management
- Navigation tools for efficient deliveries
- Receipt printing capabilities
- Earnings tracking and payout management

### Core Business Features
- **Smart Location Matching**: Customers automatically see only laundromats within their service area (typically 2 miles)
- **Flexible Service Options**: Three service types to meet different customer needs
- **Order Tracking**: QR code system ensures accurate order tracking from pickup to delivery
- **Automated Receipts**: Professional receipts printed on-site with all order details
- **Instant Communication**: Real-time notifications keep all parties informed
- **Multiple Payment Methods**: Credit card, online payment, or cash on delivery
- **Subscription Services**: Automated scheduling for regular customers

---

## User Types and Roles

### 1. Customers
**Who they are:** End users who need laundry services

**What they can do:**
- Browse and select nearby laundromats
- Place orders for pickup, delivery, or drop-off services
- Track their orders in real-time
- Manage their account information
- Set up recurring subscription services
- View order history and receipts
- Submit support requests
- Make payments through the app or cash on delivery

**Business Benefit:** Provides convenient, on-demand laundry services with full transparency and control

### 2. Laundromat Owners/Staff
**Who they are:** Business owners and employees managing laundry operations

**What they can do:**
- Manage all incoming orders
- Add new customers to the system
- Update order details (weight, pricing)
- Process drop-off orders
- Coordinate with delivery drivers
- View customer subscriptions and upcoming pickups
- Generate receipts and QR codes
- Access business analytics and reports

**Business Benefit:** Streamlined operations, better customer management, and increased efficiency

### 3. Delivery Drivers
**Who they are:** Independent contractors or employees handling pickups and deliveries

**What they can do:**
- View and accept assigned orders
- Navigate to customer locations
- Scan QR codes to verify orders
- Print receipts for customers
- Update order status
- Track earnings and completed deliveries
- Manage their profile and availability

**Business Benefit:** Clear workflow, accurate order handling, and transparent earnings tracking

### 4. System Administrators
**Who they are:** Company staff managing the overall platform

**What they can do:**
- Monitor system-wide operations
- Manage laundromat accounts
- Handle driver applications and approvals
- Configure system settings and pricing
- Generate business reports
- Manage promotions and coupons
- Oversee customer support tickets
- View analytics and business insights

**Business Benefit:** Complete control and visibility over platform operations and growth

---

## Functional Requirements by User Type

This section details all functional requirements organized by user type, specifying what each user can do within the system.

---

### Admin (System Administrator) Functional Requirements

#### 1. Dashboard and Analytics

**1.1. View System Metrics**
- View total number of subscribed clients
- View total number of new support tickets (customer, driver, laundromat)
- View pending paid bill requests
- View unpaid subscriptions count
- View credit card transfer requests
- Access real-time system statistics

**1.2. Business Analytics**
- View order statistics by area/zone
- View order statistics by date range
- View order statistics by laundromat
- View order statistics by status
- View revenue generated by orders
- Generate custom reports

#### 2. Laundromat Management

**2.1. Laundromat CRUD Operations**
- Create new laundromat accounts
- View list of all laundromats with key metrics
- View detailed laundromat profile
- Edit laundromat information
- Deactivate or activate laundromat accounts

**2.2. Laundromat Configuration**
- Set laundromat name and identification
- Configure complete address details
- Set working hours and days
- Configure pricing structure (laundry and delivery)
- Set delay rules and fees
- Configure contact information
- Set laundry status (Active, Inactive, Pending)
- Assign subscription type
- Set laundry temperature options
- Configure detergents and wash details
- Set pickup time slots
- Assign service zones

**2.3. Laundromat Analytics**
- View customer count per laundromat
- View completed orders count
- View language statistics (customer language preferences)
- View laundromat ratings
- Access order history

**2.4. Laundromat Financial Management**
- View amount owed to laundromat
- View amount owed by laundromat
- Process payments
- View outstanding balances
- Confirm received payments
- Update payment status
- Upload payment receipts
- View payment history

**2.5. Laundromat Promotions**
- Create promotions for specific laundromats
- Set promotion type (percentage, multiple orders)
- Set promotion dates
- Configure promotion details
- Assign coupon codes
- Manage promotion status

**2.6. Laundromat Customer Management**
- View all customers associated with laundromat
- Add customers to laundromat
- Remove customers from laundromat
- Enable/disable privacy mode for subscribed customers
- View customer subscription status

#### 3. Driver Management

**3.1. Driver CRUD Operations**
- Create new driver accounts
- View list of all drivers
- View detailed driver profile
- Edit driver information
- Deactivate or activate driver accounts

**3.2. Driver Registration**
- Enter driver personal information (name, DOB, ID numbers)
- Set driver type (Pickup only, Pickup and Delivery, Delivery only)
- Enter contact details
- Upload identification documents (front and back)
- Verify driver eligibility:
  - Age verification (20+ years, automated calculation)
  - Physical capability (40+ lb lifting)
  - Vehicle and insurance verification
- Enter bank account details
- Set driver address
- Select language preference
- Assign service zones
- Set driver status

**3.3. Driver Application Processing**
- View driver applications from mobile app
- Review application details
- Edit application information
- Approve or reject applications
- Update application status (New, Under Review, Approved, Pending)
- Send notifications to applicants

#### 4. Order Management

**4.1. Order Viewing and Search**
- View all orders across the platform
- Filter orders by zip code
- Filter orders by address
- Filter orders by customer name
- Filter orders by laundromat
- Filter orders by status
- Filter orders by date range
- Search orders by order ID

**4.2. Order Details**
- View complete order information
- View customer details
- View laundromat details
- View driver assignment
- View order pricing breakdown
- View order status history
- View delivery codes
- View order receipts
- View customer ratings
- View order attachments

**4.3. Order Actions**
- Assign drivers to orders
- Change driver assignments
- Send notifications to customers
- Send notifications to drivers
- Mark orders as picked up
- Mark orders as delivered
- Mark orders as completed
- Update order status
- Send delivery codes via SMS
- Add or edit order notes
- Access support chat from order

**4.4. Order Reports**
- Generate reports by area
- Generate reports by date range
- Generate reports by laundromat
- Generate reports by status
- Generate revenue reports

#### 5. Customer Management

**5.1. Customer CRUD Operations**
- Create new customer accounts
- View list of all customers
- View detailed customer profile
- Edit customer information
- View customer order history

**5.2. Customer Information**
- View customer name and contact details
- View customer address (including floor and elevator info)
- View number of associated laundromats
- View laundromat associations
- View subscription count
- View customer language preference

#### 6. Subscription Management

**6.1. Subscription CRUD Operations**
- Create new subscriptions
- View list of all subscriptions
- View subscription details
- Edit subscription information
- Delete subscriptions

**6.2. Subscription Configuration**
- Select customer (by search or manual entry)
- Set subscription type (Weekly, Bi-weekly)
- Set start date
- Configure automation (Notification or Auto-schedule)
- Set pickup day and time
- Assign to laundromat

**6.3. Subscription Monitoring**
- View customer name
- View subscription type
- View laundry day and time
- View next pickup date
- View schedule action
- View associated laundromat

#### 7. Promotions and Coupons Management

**7.1. Promotion CRUD Operations**
- Create new promotions
- View list of all promotions
- View promotion details
- Edit promotion information
- Remove promotions

**7.2. Promotion Configuration**
- Set promotion name
- Select promotion type (Percentage, Multiple orders, Coupon)
- Set start and end dates
- Select applicable laundromats
- Enter promotion details
- Assign coupon codes (if applicable)

**7.3. Coupon Management**
- Create coupon codes
- View coupon list
- Edit coupon details
- Manage coupon validity
- Track coupon usage

#### 8. Support System Management

**8.1. Customer Support**
- View all customer support tickets
- View ticket details and chat history
- Respond to customer tickets
- Send text messages
- Upload images
- Upload documents
- Send links
- Send notifications
- Update ticket status
- View related order information

**8.2. Laundromat Support**
- View all laundromat support tickets
- View ticket details and chat history
- Respond to laundromat tickets
- Send text messages
- Upload images
- Upload videos
- Send links
- Send notifications
- Update ticket status
- View related customer and order information

**8.3. Driver Support**
- View all driver support tickets
- View ticket details and chat history
- Respond to driver tickets
- Send text messages
- Upload images
- Upload videos
- Send links
- Send notifications
- Update ticket status
- View related customer, laundromat, and order information

#### 9. System Settings Management

**9.1. Subscription Pricing**
- Create subscription plan types
- Set monthly and annual pricing
- Configure promotional offers
- Set plan start and end dates
- Edit subscription plans
- Remove subscription plans

**9.2. Laundry Period Pricing**
- Create laundry service periods
- Set period names
- Configure base price per pound
- Configure app price per pound
- Edit laundry periods
- Remove laundry periods

**9.3. Delivery Pricing**
- Create delivery pricing types
- Set delivery type names
- Configure delivery prices
- Edit delivery pricing
- Remove delivery pricing

**9.4. Driver Commission**
- Create driver commission structures
- Set commission names
- Configure commission percentages
- Edit commission structures

**9.5. Pickup Scheduling**
- Create pickup time slots
- Select days of week
- Set time ranges
- Edit pickup schedules
- Remove pickup schedules

**9.6. Floor Adjustment Pricing**
- Set starting floor number
- Configure fees per additional floor
- Edit floor pricing

**9.7. Zone Management**
- Create service zones
- Set zone names
- Configure zone descriptions
- Set zone boundaries
- Edit zones
- Remove zones

**9.8. Customer Registration URL**
- View customer registration URL
- Manage registration link

#### 10. Content Management

**10.1. Rules and Regulations**
- Create rules and regulations
- Set rule title
- Select target user type (Driver, Laundromat, Customer)
- Enter rule content
- Set visibility status (Hidden/Shown)
- View all rules
- Edit rules
- Remove rules

---

### Customer (User) Functional Requirements

#### 1. Account Management

**1.1. Registration**
- Register via QR code scanning at laundromat
- Register manually in the app
- Register via SMS verification code
- Complete profile setup
- Verify phone number with OTP

**1.2. Profile Management**
- View profile information
- Edit personal information (name, email)
- Update address (including floor and elevator info)
- Change password
- Set language preference
- View account settings

**1.3. Authentication**
- Login with phone number and password
- Login with OTP verification
- Logout from account
- Recover forgotten password

#### 2. Laundromat Discovery

**2.1. View Nearby Laundromats**
- View laundromats within service zone (2 miles)
- View laundromat details (name, address, rating)
- View laundromat working hours
- View laundromat pricing
- View laundromat services offered
- View laundromat ratings and reviews

**2.2. Laundromat Selection**
- Select preferred laundromat
- View laundromat on map
- Get directions to laundromat

#### 3. Order Placement

**3.1. Pickup and Delivery Order**
- Select pickup and delivery service
- Choose preferred pickup time slot
- Enter laundry details (weight estimate, number of bags)
- Select laundry period (Regular, Express, etc.)
- Select temperature preference (Hot, Cold, Warm)
- Enter special instructions
- Review order summary
- Confirm and place order
- Receive order confirmation

**3.2. Drop-off Order**
- Create drop-off order at laundromat
- Select laundromat location
- Enter customer information
- Enter laundry details
- Select service preferences
- Generate receipt with QR code

**3.3. Delivery-Only Request**
- Request delivery for previously dropped-off laundry
- Select laundromat where laundry was dropped
- Enter receipt number
- Upload receipt photo
- Add optional notes
- Submit delivery request
- Receive confirmation

#### 4. Order Tracking

**4.1. View Orders**
- View all orders (active and completed)
- View order details
- View order status
- View order timeline
- View assigned driver information
- View laundromat information

**4.2. Order Status Updates**
- Receive real-time status updates
- View pickup confirmation
- View processing status
- View ready for delivery notification
- View delivery confirmation

**4.3. Order Information**
- View order ID and quick reference number
- View order date and time
- View service type
- View pricing breakdown
- View delivery code
- View QR code for tracking
- View receipt

#### 5. Payment Management

**5.1. Payment Options**
- Pay through app (credit card, online payment)
- Pay cash on delivery
- View payment history
- View payment receipts

**5.2. Payment Processing**
- Receive payment notifications
- View payment amount
- Confirm payment method
- Complete payment transaction
- View payment confirmation

#### 6. Subscription Management

**6.1. Create Subscription**
- Set up weekly subscription
- Set up bi-weekly subscription
- Select pickup day and time
- Choose laundromat
- Set start date
- Confirm subscription

**6.2. Manage Subscription**
- View active subscriptions
- View subscription details
- View next pickup date
- Edit subscription schedule
- Cancel subscription
- Pause subscription

#### 7. Order History

**7.1. View History**
- View all past orders
- Filter orders by date
- Filter orders by status
- View order details
- View receipts
- Download receipts

**7.2. Order Actions**
- Reorder from history
- View order tracking
- Rate and review orders
- Submit feedback

#### 8. Support and Communication

**8.1. Support Tickets**
- Create support ticket
- Link ticket to specific order
- View ticket status
- View ticket history
- Respond to support messages

**8.2. Communication**
- Receive SMS notifications
- Receive push notifications
- Receive order updates
- Receive payment notifications
- Receive delivery notifications

#### 9. Feedback and Ratings

**9.1. Order Rating**
- Rate completed orders
- Provide written feedback
- Rate laundromat service
- Rate driver service
- Submit complaints

**9.2. Feedback Management**
- View submitted feedback
- Edit feedback
- View feedback responses

---

### Driver Functional Requirements

#### 1. Account Management

**1.1. Registration and Application**
- Submit driver application through app
- Enter personal information
- Upload identification documents
- Enter vehicle information
- Enter bank account details
- Submit application for approval
- Track application status

**1.2. Profile Management**
- View driver profile
- Edit personal information
- Update contact details
- Update address
- Update vehicle information
- Update bank account details
- View assigned zones
- Update availability status

**1.3. Authentication**
- Login with credentials
- Logout from account
- Recover password

#### 2. Order Management

**2.1. View Orders**
- View assigned orders
- View order queue
- View order details
- View customer information
- View pickup location
- View delivery location
- View order status

**2.2. Order Acceptance**
- Accept new orders
- Decline orders (if applicable)
- View order requirements
- View order timeline

**2.3. Order Status Updates**
- Update order status
- Mark order as picked up
- Mark order as in transit
- Mark order as delivered
- Add delivery notes

#### 3. Pickup Process

**3.1. Pickup Workflow**
- View pickup location on map
- Navigate to pickup location
- Arrive at pickup location
- Scan QR code to verify order
- Print pickup receipt using thermal printer
- Collect laundry from customer
- Confirm pickup completion
- Update pickup status

**3.2. Pickup Receipt**
- Generate pickup receipt
- Print receipt with QR code
- Receipt includes:
  - Order details
  - Customer information
  - QR code for tracking
  - Pickup timestamp

#### 4. Delivery Process

**4.1. Delivery Workflow**
- View delivery location on map
- Navigate to delivery location
- Arrive at delivery location
- Scan QR code to verify customer
- Verify delivery code
- Collect payment (if cash on delivery)
- Deliver clean laundry
- Print delivery receipt
- Confirm delivery completion
- Update delivery status

**4.2. Delivery Receipt**
- Generate delivery receipt
- Print receipt with QR code
- Receipt includes:
  - Order details
  - Customer information
  - Payment information
  - Delivery timestamp

#### 5. QR Code Operations

**5.1. QR Code Scanning**
- Scan QR code at pickup
- Scan QR code at delivery
- Verify order details
- Verify customer identity
- Confirm correct order matching

**5.2. QR Code Verification**
- Verify QR code validity
- View order information from QR code
- Confirm order details match

#### 6. Navigation and Location

**6.1. Location Services**
- View customer locations on map
- Get directions to pickup location
- Get directions to delivery location
- View current location
- Track route progress

#### 7. Earnings and Financial Management

**7.1. Earnings Tracking**
- View total earnings
- View earnings by period
- View completed orders count
- View earnings breakdown
- View commission details

**7.2. Payout Management**
- View payout history
- Request payout
- Track payout status
- View bank account details

#### 8. Communication

**8.1. Notifications**
- Receive new order notifications
- Receive order update notifications
- Receive payment notifications
- Receive system notifications

**8.2. Support**
- Create support tickets
- View support ticket status
- Communicate with support team
- Upload images for support
- Upload videos for support

#### 9. Order History

**9.1. View History**
- View completed orders
- View order details
- View earnings per order
- Filter orders by date
- View order statistics

---

### Vendor (Laundromat) Functional Requirements

#### 1. Account Management

**1.1. Registration and Setup**
- Register laundromat account
- Complete business profile
- Set up business information
- Configure service offerings
- Set pricing structure

**1.2. Profile Management**
- View business profile
- Edit business information
- Update contact details
- Update address
- Update working hours
- Update pricing
- Update service offerings

**1.3. Authentication**
- Login to vendor dashboard/tablet app
- Logout from account
- Recover password

#### 2. Order Management

**2.1. View Orders**
- View all orders for laundromat
- View orders by status (Pending, In Progress, Completed)
- View new orders
- View order queue
- View order details
- Filter orders by date
- Filter orders by customer
- Filter orders by status

**2.2. Order Processing**
- Accept new orders
- Update order status
- Add laundry weight
- Update order pricing
- Add order notes
- Assign drivers to orders
- Mark orders as in progress
- Mark orders as completed
- Mark orders as ready for delivery

**2.3. Order Details**
- View customer information
- View order specifications
- View laundry details
- View pricing information
- View driver assignment
- View delivery information

#### 3. Customer Management

**3.1. Customer CRUD**
- Add new customers
- View customer list
- Search customers by phone number
- View customer details
- Edit customer information
- View customer order history

**3.2. Customer Registration**
- Register customers at drop-off
- Enter customer information
- Send SMS verification code
- Complete customer registration
- Link customer to orders

**3.3. Subscribed Customers**
- View subscribed customers list
- View customer initials (privacy mode)
- View order frequency
- View next scheduled pickups
- Manage subscription schedules

#### 4. Drop-off Order Creation

**4.1. Create Drop-off Order**
- Create order when customer drops off laundry
- Select or add customer
- Enter laundry weight
- Select laundry period
- Select temperature preference
- Enter special instructions
- Calculate pricing
- Generate receipt with QR code
- Print receipt

**4.2. Order Configuration**
- Set service type
- Set laundry period
- Set temperature
- Add notes
- Set pricing

#### 5. Delivery Request Processing

**5.1. View Delivery Requests**
- View all delivery-only requests
- View request details
- View receipt images
- Verify receipt numbers

**5.2. Process Delivery Request**
- Verify customer receipt
- Update order weight
- Update order pricing
- Assign driver
- Notify customer of cost
- Confirm delivery request

#### 6. QR Code Management

**6.1. QR Code Generation**
- Generate QR codes for orders
- Print receipts with QR codes
- View QR code information

**6.2. QR Code Scanning**
- Scan QR codes to verify orders
- Verify order details
- Confirm order matching

#### 7. Subscription Management

**7.1. View Subscriptions**
- View all customer subscriptions
- View subscription details
- View subscription schedules
- View next pickup dates

**7.2. Subscription Operations**
- Create subscriptions for customers
- Edit subscription schedules
- View subscription statistics
- Manage subscription status

#### 8. Dashboard and Analytics

**8.1. Business Dashboard**
- View total orders
- View new orders
- View orders in progress
- View completed orders
- View canceled orders
- View total revenue
- View average rating

**8.2. Subscribed Customer Analytics**
- View total subscribed customers
- View total subscription orders
- View current month orders
- View subscription performance

#### 9. Billing and Payment

**9.1. Financial Overview**
- View amount owed to laundromat
- View amount owed by laundromat
- View payment status
- View recent payments
- View payment history

**9.2. Payment Processing**
- Confirm payment received
- Upload payment receipts
- Update payment status
- View outstanding balances

#### 10. Support and Communication

**10.1. Support Tickets**
- Create support tickets
- View ticket status
- Communicate with support team
- Upload images
- Upload videos
- Receive support responses

**10.2. Communication**
- Send notifications to customers
- Send notifications to drivers
- Receive order notifications
- Receive system notifications

#### 11. Receipt and Documentation

**11.1. Receipt Generation**
- Generate receipts for orders
- Print receipts
- View receipt history
- Download receipts

**11.2. Order Documentation**
- Upload order confirmation photos
- View order attachments
- Manage order documents

---

## System Dashboard (Admin Panel)

The System Dashboard provides administrators with a comprehensive overview of the entire platform's operations, enabling quick decision-making and efficient management.

### 1. Dashboard Home (Executive Summary)

The dashboard home displays key business metrics at a glance, allowing administrators to quickly assess the health and activity of the platform.

#### 1.1. Key Performance Indicators

**Subscribed Clients**
- Shows the total number of customers with active subscription plans
- **Business Value:** Indicates customer retention and recurring revenue potential

**New Support Tickets**
- Displays the total number of new support requests from customers, drivers, and laundromats
- **Business Value:** Helps prioritize customer service needs and identify systemic issues

**Pending Payment Requests**
- Shows credit card payments awaiting approval
- **Business Value:** Ensures timely payment processing and cash flow management

**Unpaid Subscriptions**
- Identifies subscriptions that haven't been paid in the current billing cycle
- **Business Value:** Helps identify payment issues and maintain subscription revenue

**Transfer Requests**
- Displays payout requests from laundromats and drivers
- **Business Value:** Manages financial transactions and ensures timely payouts

### 2. Laundromat Management

Administrators can manage all laundromat partners through this comprehensive section, ensuring quality service delivery and business growth.

#### 2.1. Laundromat Directory

**2.1.1. Laundromat List View**
The list provides a quick overview of all laundromat partners with key business metrics:
- **Date Added**: When the laundromat joined the platform
- **Customer Count**: Number of unique customers served
- **Active Status**: Whether the laundromat is currently operational
- **Completed Orders**: Total successful orders processed
- **Location**: City for geographic organization
- **Quick Actions**: Edit, View details, or Add new laundromat

**Business Value:** Enables quick assessment of partner performance and operational status

**2.1.2. Laundromat Profile View**
Complete business profile of each laundromat partner:

**Business Information:**
- Laundromat name and unique identifier
- Complete address details (street, city, state, zip code, additional details)
- Service area (Zone assignment)
- Operational status (Active, Inactive, Pending approval)

**Service Details:**
- Working hours and availability
- Service pricing structure (laundry pricing, delivery fees)
- Delay policies and associated fees
- Laundry temperature options (Hot, Cold, Warm)
- Detergent and washing preferences
- Subscription plan type (Basic, Premium)

**Customer Insights:**
- Customer rating and reviews
- **Language Analytics**: Shows which languages customers use when placing orders
  - Language names and usage percentages
  - Helps understand customer demographics

**Quick Access:**
- Direct link to view all orders for this laundromat
- Direct link to view all customers associated with this laundromat

**Business Value:** Complete visibility into partner operations, service quality, and customer preferences

**2.1.3. Onboard New Laundromat Partner**
When adding a new laundromat to the platform, administrators collect comprehensive business information:

**Basic Information:**
- Business name
- Complete address (street, city, state, zip code, additional location details)
- Service zone assignment (determines which customers can see this laundromat)

**Operating Schedule:**
- Days of operation
- Operating hours for each day
- Pickup time slots available

**Pricing Structure:**
- Laundry service pricing (select from predefined periods or create custom)
  - Can set different prices for different service types (e.g., regular wash, express, dry clean)
  - Price per pound for each service type
- Delivery pricing (use system defaults or set custom rates)

**Business Policies:**
- Delay policies (maximum days for order completion)
- Delay fees (charges for late orders)
- Laundry temperature options offered
- Detergent and washing preferences

**Contact Information:**
- Primary contact person (name, position)
- Email and phone number
- Preferred communication method (Call, Text, or Email)

**Service Configuration:**
- Account status (Active, Inactive, or Pending activation)
- Subscription plan type
- Service capabilities

**Business Value:** Ensures new partners are properly configured with accurate pricing and policies before going live

**2.1.4. Update Laundromat Information**
All business information can be updated at any time to reflect changes in:
- Pricing adjustments
- Operating hours
- Service offerings
- Contact information
- Business policies

**Business Value:** Maintains accurate partner information and ensures customers receive correct service details

**2.1.5. Financial Management**
Comprehensive billing and payment tracking for each laundromat:

**Financial Overview:**
- Amount owed to laundromat (platform owes the partner)
- Amount owed by laundromat (partner owes the platform)
- Payment method preferences (Online transfers or Cash)

**Payment Processing:**
- View all outstanding balances
- Confirm when payments are received
- Update payment status
- Upload payment receipts for record-keeping

**Business Value:** Ensures accurate financial tracking and timely settlements with partners

**2.1.6. Promotional Campaigns**
Create targeted promotions for specific laundromats to drive business:

**Promotion Setup:**
- Promotion type (Percentage discount or Multiple orders discount)
- Campaign duration (start and end dates)
- Promotion details and terms
- Optional coupon codes for tracking

**Business Value:** Enables marketing campaigns to increase customer engagement and order volume

**2.1.7. Customer Management**
View and manage all customers associated with a specific laundromat:

**Customer List:**
- View all customers who have used this laundromat
- Add new customers manually
- Remove customers if needed

**Privacy Protection:**
- **Privacy Mode**: When enabled, subscribed customers are shown only by their initials
- Protects customer privacy while allowing laundromats to manage subscriptions

**Business Value:** Helps laundromats maintain customer relationships while respecting privacy

### 3. Promotions and Coupons Management

A centralized system for creating and managing marketing campaigns across the platform.

#### 3.1. Promotions Management

**View All Promotions:**
- See all active and scheduled promotions
- Monitor promotion performance
- Track which laundromats are participating

**Create New Promotion:**
- **Promotion Name**: Clear, descriptive name for the campaign
- **Promotion Type**:
  - Percentage discount (e.g., 20% off)
  - Multiple orders discount (e.g., buy 3 get 1 free)
  - Coupon-based promotion
- **Campaign Period**: Start and end dates
- **Target Laundromats**: Select which laundromats can participate
- **Promotion Details**: Terms and conditions
- **Coupon Codes**: Optional tracking codes for analytics

**Manage Promotions:**
- Edit existing promotions
- Deactivate or remove promotions
- Monitor promotion effectiveness

**Business Value:** Enables strategic marketing to increase customer acquisition and retention

### 4. Driver Management

Comprehensive management of the delivery driver network, ensuring quality service delivery and proper vetting.

#### 4.1. Driver Directory

**4.1.1. Driver List Overview**
Quick view of all drivers with essential information:
- Driver name and identification
- Service capabilities (Pickup only, Pickup and Delivery, or Delivery only)
- Contact information
- Assigned service zone
- Current status (Active or Inactive)
- Language preferences

**Business Value:** Enables efficient driver assignment and ensures adequate coverage in all service areas

**4.1.2. Onboard New Driver**
Comprehensive driver registration process ensures quality and compliance:

**Personal Information:**
- Full name (First and Last)
- Date of Birth (system automatically calculates age)
- Government ID numbers (State ID, Social Security Number)

**Service Capabilities:**
- Service type selection (Pickup only, Pickup and Delivery, or both)
- Assigned service zone
- Language preferences

**Verification Requirements:**
- Photo ID upload (front and back)
- **Eligibility Checks:**
  - Age verification (must be 20 years or older - automatically calculated)
  - Physical capability (can lift 40+ pounds)
  - Vehicle ownership and insurance confirmation

**Payment Information:**
- Bank account details (Account number and Routing number)
- Required for driver payouts

**Contact Information:**
- Phone number and email address
- Physical address

**Account Status:**
- Set initial status (Active, Inactive, or Pending)

**Business Value:** Ensures only qualified, verified drivers join the platform, maintaining service quality and safety standards

**4.1.3. Update Driver Information**
All driver information can be updated to reflect:
- Contact information changes
- Service zone reassignments
- Status changes (activate/deactivate)
- Payment information updates

**Business Value:** Maintains accurate driver records and ensures proper service coverage

**4.1.4. Driver Profile View**
Complete view of driver information including:
- Personal details
- Service history
- Performance metrics
- Earnings summary
- Current assignments

**Business Value:** Provides comprehensive view for performance evaluation and support

**4.1.5. Driver Application Processing**
When drivers apply through the mobile app, administrators can:

**Application Management:**
- View all pending applications
- Review application details
- Edit application information if needed

**Approval Process:**
- Approve qualified applicants
- Reject applications that don't meet requirements
- Update application status (New, Under Review, Approved, Pending)

**Communication:**
- Send notifications to applicants about their status
- Provide feedback and next steps

**Business Value:** Streamlines driver onboarding while maintaining quality standards

### 5. Scheduled Laundry Subscriptions

Manage recurring laundry service subscriptions for regular customers, ensuring consistent revenue and customer satisfaction.

#### 5.1. Subscription Management

**5.1.1. Active Subscriptions Overview**
View all active subscriptions with key information:
- Customer name
- Subscription frequency (Weekly or Bi-weekly)
- Scheduled pickup day and time
- Next scheduled pickup date
- Automation setting (Notification only or Auto-schedule orders)
- Assigned laundromat

**Business Value:** Provides visibility into recurring revenue and helps plan operations

**5.1.2. Create New Subscription**
Set up recurring service for customers:

**Subscription Details:**
- Select customer (search by name or phone)
- Choose subscription type (Weekly or Bi-weekly)
- Set start date
- Configure automation (Send notifications or automatically create orders)
- Set preferred pickup day and time
- Assign to specific laundromat

**Business Value:** Enables predictable revenue streams and improves customer retention

**5.1.3. Modify Subscriptions**
Update existing subscriptions to accommodate:
- Schedule changes
- Frequency adjustments
- Laundromat reassignments
- Automation preferences

**Business Value:** Maintains customer satisfaction by accommodating changing needs

### 6. Order Management

Centralized system for viewing, managing, and analyzing all orders across the platform.

#### 6.1. Order Search and Filtering

Administrators can quickly find specific orders using multiple filters:
- **By Location**: Zip code or address
- **By Customer**: Customer name search
- **By Laundromat**: Filter orders by specific laundromat
- **By Status**: View orders in different stages (Pending, In Progress, Completed, etc.)
- **By Date Range**: Analyze orders within specific time periods

**Business Value:** Enables quick problem resolution and business analysis

#### 6.2. Order List View

Comprehensive list showing all orders with essential information:
- Customer name
- Order date and time
- Service type (Pickup, Delivery, Drop-off)
- Current order status
- Assigned driver (if any)
- Quick actions (View details or Edit)

**Business Value:** Provides complete visibility into all platform activity

#### 6.3. Order Details and Management

**6.3.1. Complete Order Information**
Full view of every order including:

**Customer Information:**
- Name, address, and phone number
- Customer language preference

**Order Details:**
- Order date and time
- Service type (Pickup, Delivery, or Drop-off)
- Laundromat assigned
- Laundry service period selected
- Temperature preference
- Current status in workflow

**Service Delivery:**
- Driver assigned (if any)
- Delivery code for customer verification

**Financial Information:**
- Total order price (laundry + delivery)
- Driver commission (when applicable, e.g., for multi-floor deliveries)

**Order Documentation:**
- Receipt information
- Customer rating and feedback
- Order confirmation photos

**Business Value:** Complete order visibility enables quality control and customer service excellence

**6.3.2. Order Status Management**
Update order status as it progresses through the service workflow:
- Pending → Confirmed → In Progress → Completed → Delivered

**Business Value:** Ensures accurate order tracking and timely service delivery

**6.3.3. Delivery Verification**
View and manage delivery codes used for customer verification at delivery

**Business Value:** Ensures secure and accurate order delivery

**6.3.4. Customer Support Integration**
Direct access to support chat for any order-related issues

**Business Value:** Enables quick resolution of customer concerns

**6.3.5. Order Notes**
Add internal notes about special instructions, issues, or customer preferences

**Business Value:** Improves service quality through better communication

#### 6.4. Order Management Actions

Administrators can take various actions to manage orders effectively:

**Driver Management:**
- Assign a driver to an order
- Change driver assignment if needed

**Communication:**
- Send notifications to customers about order status
- Send notifications to drivers about new assignments
- Send delivery codes via SMS to customers

**Status Updates:**
- Mark orders as picked up
- Mark orders as delivered
- Mark orders as completed
- Update any order status as needed

**Business Value:** Ensures smooth order fulfillment and keeps all parties informed

#### 6.5. Business Analytics and Reporting

Comprehensive reporting tools for business intelligence:

**Geographic Analysis:**
- Order volume by service area
- Helps identify high-demand locations

**Time-Based Analysis:**
- Orders by date range
- Seasonal trends and patterns

**Performance Metrics:**
- Orders by laundromat (partner performance)
- Orders by status (operational efficiency)
- Revenue generated by orders (financial performance)

**Business Value:** Enables data-driven decision making for growth and optimization

### 6.6. Customer Management

Centralized customer database for relationship management and analytics.

**6.6.1. Customer Directory**
View all platform customers with key information:
- Customer name and contact information (phone, email)
- Number of laundromats they've used
- Details of associated laundromats
- Number of active subscriptions

**6.6.2. Add New Customer**
Manually add customers to the system with:
- Name
- Phone number
- Email address
- Complete address (including floor and elevator information for accurate delivery)

**Business Value:** Enables customer onboarding when needed and maintains complete customer records

**6.6.3. Customer Profile View**
Complete customer information including:
- Contact details
- Service history (number of laundromats used)
- Active subscriptions count
- Complete address information
- Language preference

**Business Value:** Provides comprehensive customer insights for personalized service and marketing

### 7. Customer Support System

Comprehensive support ticket management for all user types, ensuring timely resolution of issues and excellent customer service.

#### 7.1. Customer Support Tickets

**7.1.1. Support Ticket List**
View all customer support requests with:
- Customer name
- Ticket creation time
- Issue type/category
- Current status
- Quick access to view or manage ticket

**Business Value:** Enables efficient support queue management and ensures no customer issues are overlooked

**7.1.2. Support Chat Interface**
Interactive communication tool for resolving customer issues:

**Communication Features:**
- View complete chat history
- Send text messages
- Share images (screenshots, photos)
- Share documents
- Send helpful links
- Send push notifications

**Context Information:**
- Customer name and details
- Ticket creation time
- Related laundromat (if applicable)
- Related order (if applicable)

**Business Value:** Provides efficient, context-rich communication for quick issue resolution

#### 7.2. Laundromat Partner Support

**7.2.1. Partner Support List**
View all support requests from laundromat partners:
- Laundromat name
- Ticket creation time
- Issue type
- Status
- Quick access to manage ticket

**Business Value:** Ensures partner satisfaction and operational efficiency

**7.2.2. Partner Support Chat**
Enhanced communication with video support:
- Complete chat history
- Text messaging
- Image sharing
- Video sharing (for complex issues)
- Link sharing
- Push notifications
- Context: Laundromat details, related customer, related order

**Business Value:** Enables comprehensive support for business partners

#### 7.3. Driver Support

**7.3.1. Driver Support List**
View all support requests from delivery drivers:
- Driver name
- Ticket creation time
- Issue type
- Status
- Quick access to manage ticket

**Business Value:** Maintains driver satisfaction and operational support

**7.3.2. Driver Support Chat**
Full-featured support for drivers:
- Complete chat history
- Text messaging
- Image sharing
- Video sharing (for delivery issues)
- Link sharing
- Push notifications
- Context: Driver details, related customer, related laundromat, related order

**Business Value:** Ensures drivers have the support they need for successful deliveries

### 8. System Configuration

Centralized settings management for platform-wide policies, pricing, and operational parameters.

#### 8.1. Subscription Plan Management
Configure subscription offerings for customers:

**Create Subscription Plans:**
- Plan name
- Pricing (Monthly and Annual options)
- Promotional offers (e.g., first month free)
- Active period (start and end dates)
- Multiple plans can be created

**Manage Plans:**
- View all subscription plans
- Edit existing plans
- Deactivate or remove plans

**Business Value:** Enables flexible subscription offerings to attract and retain customers

#### 8.2. Service Pricing Configuration
Set up laundry service pricing options:

**Create Service Periods:**
- Service period name (e.g., Regular, Express, Deluxe)
- Base price per pound (standard pricing)
- App price per pound (pricing for app orders)
- Multiple service periods can be configured

**Manage Pricing:**
- View and edit all service periods
- Adjust pricing as needed

**Business Value:** Provides flexible pricing options to meet different customer needs and market conditions

#### 8.3. Delivery Fee Structure
Configure delivery pricing:

**Create Delivery Types:**
- Delivery type name
- Associated delivery fee
- Multiple delivery types can be created

**Manage Delivery Pricing:**
- View and edit delivery fees
- Adjust based on market conditions

**Business Value:** Ensures delivery pricing remains competitive and profitable

#### 8.4. Driver Commission Structure
Set driver payment percentages:

**Configure Commissions:**
- Commission tier name
- Percentage rate for drivers
- Can create multiple commission structures

**Business Value:** Ensures fair and competitive driver compensation

#### 8.5. Pickup Schedule Configuration
Set available pickup time slots:

**Create Pickup Windows:**
- Select days of the week
- Set time ranges for each day
- Multiple time slots can be configured

**Business Value:** Ensures customers have convenient pickup options while optimizing driver schedules

#### 8.6. Multi-Floor Delivery Pricing
Configure additional fees for deliveries to upper floors:

**Floor Pricing:**
- Set starting floor number (e.g., deliveries above 2nd floor incur fees)
- Set fee amount per additional floor

**Business Value:** Fairly compensates drivers for more challenging deliveries

#### 8.7. Customer Registration Link
View and manage the URL used for customer registration

**Business Value:** Enables marketing campaigns and customer acquisition

#### 8.8. Service Zone Management
Define geographic service areas:

**Zone Configuration:**
- Zone name
- Zone description
- Geographic boundaries

**Business Value:** Ensures customers are matched with appropriate nearby laundromats

### 9. Content Management

#### 9.1. Rules and Regulations

Manage platform policies and terms of service for different user types.

**9.1.1. Rules Directory**
View all published rules and regulations:
- Content name and title
- Author (who created it)
- Publication date
- Target audience (Drivers, Laundromats, or Customers)
- Visibility status (Hidden or Shown to users)

**Business Value:** Ensures users are informed about platform policies and terms

**9.1.2. Create New Rules**
Add new policies or update existing ones:
- Rule title
- Target user type
- Full content/text
- Visibility setting (immediately show or keep hidden until ready)

**Business Value:** Maintains clear communication of platform policies and updates

---

## Laundromat Dashboard

The Laundromat Dashboard provides business owners with a comprehensive view of their operations, enabling data-driven decisions and efficient management.

### 1. Business Overview Dashboard

#### 1.1. Key Performance Indicators
The dashboard displays essential business metrics at a glance:

**Order Metrics:**
- **Total Orders**: Complete count of all orders processed
- **New Orders**: Recently received orders requiring attention
- **Orders in Progress**: Currently being processed
- **Completed Orders**: Successfully finished orders
- **Canceled Orders**: Cancelled order count

**Financial Metrics:**
- **Total Revenue**: Total income generated
- **Average Order Rating**: Customer satisfaction score

**Business Value:** Provides immediate insight into business health and performance trends

### 2. Order Management

Complete order management system for laundromat operations.

#### 2.1. Order Processing

**2.1.1. Order Queue**
View all orders with essential information:
- Order identification number
- Customer name
- Order date and time
- Service type (Pickup, Delivery, or Drop-off)
- Current processing status
- Assigned driver (if applicable)
- Order total price
- Quick actions (View full details or Edit)

**Business Value:** Enables efficient order processing and prioritization

**2.1.2. Order Details and Processing**
Complete order information for processing:
- Customer contact information (name, address, phone)
- Order timing (date and time)
- Service specifications (type, temperature preference)
- Current status
- Order verification code
- Driver assignment details
- Special instructions or notes
- Customer feedback and ratings

**Business Value:** Ensures accurate order fulfillment and customer satisfaction

### 3. Subscribed Customer Management

A privacy-focused view of subscription customers that balances business needs with customer privacy protection.

#### 3.1. Subscription Overview

**3.1.1. Total Subscribed Customers**
Shows the total number of customers with active subscription plans.

**Business Value:** Indicates recurring revenue base and customer loyalty

**3.1.2. Total Subscription Orders**
Displays total orders from subscribed customers over selected time periods (monthly, quarterly, or annually).

**Business Value:** Measures subscription program effectiveness

**3.1.3. Current Month Activity**
Shows orders from subscribed customers in the current month.

**Business Value:** Provides real-time view of subscription program performance

#### 3.2. Subscription Customer List

A privacy-protected view that allows laundromats to manage subscriptions while protecting customer information.

**3.2.1. Customer Identification**
Customers are shown by initials only (e.g., A.B., J.D.) to protect privacy.

**3.2.2. Order Activity**
Shows order frequency for each customer (e.g., "3 orders this month").

**3.2.3. Upcoming Pickups**
Displays the next scheduled pickup date for each customer.

**Business Value:** Enables effective subscription management while maintaining customer privacy and trust

### 4. Financial Management

#### 4.1. Billing Overview
Complete financial tracking for laundromat operations:
- Amount owed to laundromat (platform payments)
- Amount owed by laundromat (platform fees)
- Payment status tracking
- Recent payment history
- Complete payment history

**Business Value:** Ensures accurate financial tracking and timely settlements

#### 4.2. Payment Processing
Manage incoming and outgoing payments:
- Confirm when payments are received
- Upload payment receipts for record-keeping
- Update payment status

**Business Value:** Maintains accurate financial records and ensures proper cash flow

### 5. Customer Support Integration

#### 5.1. Support Ticket System
Integrated support system for customer assistance.

**5.1.1. Customer Support Requests**
Customers can create support tickets for:
- Order-related issues
- General inquiries
- Service questions

**5.1.2. Admin Escalation**
All support tickets are routed to system administrators for:
- Professional handling
- Consistent resolution
- Quality assurance

**Business Value:** Ensures customers receive timely, professional support while maintaining service quality standards

---

## Customer Mobile Application

The customer mobile app provides a convenient, user-friendly interface for accessing laundry services anytime, anywhere.

### Service Options

#### 1. Pickup and Delivery Service
Complete full-service laundry solution - customers request both pickup and delivery.

**How It Works:**
- Customer selects preferred pickup time from available slots (e.g., 12:00 PM, 3:00 PM, 7:00 PM)
- Driver arrives at scheduled time with thermal printer
- Driver prints receipt with QR code and order details
- Laundromat processes laundry and updates weight/cost
- Customer receives notification with final cost
- Customer pays through app or cash on delivery
- Driver delivers clean laundry and scans QR code for verification

**Customer Benefits:** Complete convenience - no need to leave home, professional service, secure tracking

#### 2. Delivery-Only Service
For customers who drop off laundry but later want it delivered.

**How It Works:**
- Customer selects the laundromat where they dropped off laundry
- Customer enters receipt number from drop-off
- Customer uploads photo of receipt
- Laundromat verifies order and updates weight/cost
- Customer receives notification with delivery cost
- Customer pays through app or cash on delivery
- Driver is assigned and delivers laundry
- QR code verification at delivery

**Customer Benefits:** Flexibility to add delivery service after drop-off, easy receipt verification

#### 3. Laundromat-Initiated Delivery
When customers drop off laundry at the laundromat, staff can set up delivery service.

**How It Works:**
- Customer drops off laundry at laundromat
- Staff adds customer to system
- Customer receives SMS with 4-digit verification code
- Customer can also self-register by scanning QR code at laundromat
- Staff enters laundry weight and service details
- System automatically calculates pricing
- Customer receives SMS with order details and app download link
- Customer can track order through app
- Driver delivers with QR code verification

**Customer Benefits:** Easy registration, automatic price calculation, full order tracking

### Customer Registration and Account Setup

**Registration Options:**
1. **QR Code Registration**: Scan QR code at laundromat, receive verification code via SMS
2. **Manual Registration**: Enter information directly in the app
3. **Staff-Assisted Registration**: Laundromat staff adds customer during drop-off
4. **SMS Verification**: Receive 4-digit code via SMS for phone verification

**Customer Benefits:** Multiple convenient registration methods ensure easy account setup

### Key Customer Features

**Smart Location Services:**
- Automatically shows only nearby laundromats (within 2 miles)
- Ensures convenient service access

**Real-Time Order Tracking:**
- Live order status updates
- Know exactly where your laundry is in the process

**Flexible Payment Options:**
- Pay securely through the app
- Or pay cash when driver delivers

**Subscription Services:**
- Set up weekly or bi-weekly automatic pickups
- Never forget to schedule laundry service

**Order History:**
- View all past orders
- Access receipts anytime

**Customer Support:**
- Create support tickets for any questions or issues
- Get help when you need it

**Multi-Language Support:**
- App available in multiple languages
- Comfortable experience for all customers

---

## Driver Mobile Application

The driver app provides delivery professionals with all the tools needed for efficient, accurate order fulfillment.

### Core Functionality

#### 1. Order Management
**Order Dashboard:**
- View all assigned orders
- Accept or decline new orders
- Update order status as work progresses
- Access complete order and customer information

**Driver Benefits:** Clear workflow, easy order management, complete information access

#### 2. Pickup Workflow
**Pickup Process:**
- Navigate to customer pickup location using integrated maps
- Scan QR code to verify correct order
- Print professional receipt using thermal printer
- Confirm pickup completion in app

**Driver Benefits:** Accurate order handling, professional customer interaction, streamlined process

#### 3. Delivery Workflow
**Delivery Process:**
- Navigate to customer delivery location
- Scan QR code to verify correct customer and order
- Collect payment if customer pays cash
- Confirm delivery completion
- Print delivery receipt for customer

**Driver Benefits:** Ensures accurate deliveries, secure payment collection, professional service

#### 4. QR Code Verification System
**Order Verification:**
- Scan QR codes at both pickup and delivery
- Verify order details match
- Ensure correct items go to correct customer

**Driver Benefits:** Eliminates errors, protects driver and customer, ensures quality service

#### 5. Receipt Printing
**Professional Receipts:**
- Print receipts at pickup and delivery
- Receipts include:
  - Complete order details
  - Customer information
  - QR code for tracking
  - Payment information

**Driver Benefits:** Professional service delivery, customer satisfaction, accurate records

#### 6. Earnings and Financial Management
**Financial Tracking:**
- View total earnings
- See completed order count
- Track payout requests and status

**Driver Benefits:** Transparent earnings, easy financial management, payment tracking

#### 7. Profile and Settings
**Account Management:**
- Update personal information
- View assigned service zones
- Manage vehicle details

**Driver Benefits:** Easy account management, zone awareness, profile control

### Driver Requirements

To ensure quality service and safety, all drivers must meet these requirements:
- **Age Requirement**: Must be 20 years or older (automatically verified from date of birth)
- **Physical Capability**: Must be able to lift up to 40 pounds
- **Vehicle Requirement**: Must own a vehicle with valid insurance

---

## Vendor Tablet Application

The vendor tablet app is designed for laundromat staff to manage daily operations efficiently using tablet devices.

### Core Operational Features

#### 1. Order Processing
**Complete Order Management:**
- View all orders organized by status (Pending, In Progress, Completed)
- Update order status as work progresses
- Add laundry weight and calculate pricing
- Assign drivers to orders
- Access complete order details

**Business Value:** Streamlined order processing, efficient workflow management

#### 2. Customer Relationship Management
**Customer Database:**
- Add new customers to the system
- View complete customer list
- Search customers quickly by phone number
- View individual customer order history
- Manage customer subscription plans

**Business Value:** Better customer service, relationship building, subscription revenue management

#### 3. Drop-off Service Processing
**In-Store Order Creation:**
When customers bring laundry to the laundromat:
- Create new order in system
- Add or select customer information
- Enter laundry weight
- Select service type and temperature preference
- Generate professional receipt with QR code

**Business Value:** Efficient in-store service, accurate order creation, professional receipts

#### 4. Delivery Request Handling
**Process Customer Delivery Requests:**
When customers request delivery via app:
- View all delivery requests
- Verify customer receipt numbers and uploaded images
- Update order weight and final pricing
- Assign appropriate driver
- Notify customer of final cost

**Business Value:** Additional revenue opportunity, customer convenience, service expansion

#### 5. QR Code System
**Order Tracking and Verification:**
- Generate unique QR codes for each order
- Print receipts with embedded QR codes
- Scan QR codes to verify orders

**Business Value:** Accurate order tracking, error prevention, professional service

#### 6. Subscription Program Management
**Recurring Customer Management:**
- View all subscribed customers
- Manage subscription schedules and preferences
- See upcoming pickup dates
- Plan operations around scheduled pickups

**Business Value:** Predictable revenue, customer retention, operational planning

#### 7. Business Dashboard
**Performance Overview:**
- View order volume statistics
- Track revenue trends
- Monitor completed orders
- Review pending orders requiring attention

**Business Value:** Data-driven decision making, performance monitoring, business insights

---

## Order Management Workflows

The system supports multiple order types to meet different customer needs and business scenarios.

### Order Service Types

1. **Pickup & Delivery**: Complete full-service - driver picks up dirty laundry and delivers clean laundry
2. **Drop-off**: Customer brings laundry to laundromat, picks up when ready
3. **Delivery-Only**: Customer drops off laundry, then requests delivery service
4. **Subscription Orders**: Automated recurring orders for regular customers

### Order Lifecycle

Every order progresses through these stages:
- **Pending**: Order placed, awaiting confirmation
- **Confirmed**: Order confirmed and scheduled
- **In Progress**: Laundry being processed
- **Completed**: Laundry finished, ready for delivery
- **Delivered**: Successfully delivered to customer

### Order Information

Each order contains complete information for accurate processing:

**Identification:**
- Unique order ID
- Quick reference number

**Party Information:**
- Customer details (name, address, phone, email)
- Laundromat information
- Driver assignment (when applicable)

**Service Details:**
- Service type
- Laundry weight and bag count
- Temperature preference
- Service period selected
- Customer language preference

**Financial Information:**
- Laundry service price
- Delivery fee
- Total order amount
- Payment method and status

**Tracking and Verification:**
- QR code for order tracking
- Delivery code for customer verification
- Order timestamps (created, picked up, delivered)

### Pricing Structure

**Service Pricing:**
- Laundry price calculated by weight and service type
- Delivery price based on number of bags and delivery type
- Additional fees for multi-floor deliveries (above specified floor)
- Delay fees for late pickups or deliveries (if applicable)
- Driver commission for challenging deliveries (multi-floor)

**Business Value:** Transparent, fair pricing that compensates all parties appropriately

---

## Customer Support System

A comprehensive support system ensures all users receive timely, effective assistance when needed.

### Support Channels

**1. Customer Support**
- Customers can create support tickets for any questions or issues
- Tickets can be linked to specific orders for context
- All tickets managed by system administrators for professional resolution

**2. Laundromat Partner Support**
- Laundromat staff can request assistance for operational issues
- Technical support for app usage
- Business support for account management

**3. Driver Support**
- Drivers can get help with delivery issues
- App technical support
- Account and payment questions

### Communication Tools

**Rich Communication Features:**
- Text messaging for quick communication
- Image sharing for visual problem description
- Document sharing for detailed information
- Video sharing (for partners and drivers) for complex issues
- Link sharing for helpful resources
- Push notifications for instant updates
- Complete chat history for reference

**Business Value:** Ensures all users have access to professional support, improving satisfaction and retention

### Support Ticket Lifecycle

Tickets progress through these stages:
- **New**: Just created, awaiting review
- **Pending**: Assigned and awaiting response
- **Under Review**: Being actively investigated
- **Resolved**: Issue resolved, awaiting confirmation
- **Closed**: Ticket completed and archived

---

## System Features Summary

### Complete Feature Set

The Soft Laundry Delivery System includes a comprehensive set of features designed to support all aspects of the laundry service business:

**Administrative Features:**
- Complete system dashboard with key business metrics
- Full laundromat partner management
- Comprehensive driver management and application processing
- Complete order lifecycle management
- Customer database with privacy protection features
- Subscription program management (weekly and bi-weekly)
- Promotions and coupon management system
- Multi-channel support system (customers, partners, drivers)
- Complete system configuration and settings management

**Operational Features:**
- QR code tracking system for accurate order management
- Thermal receipt printing for professional service
- Customer language preference tracking
- Smart zone-based laundromat matching
- Multiple payment method integration
- Complete billing and financial management system

**Business Intelligence:**
- Order statistics and analytics
- Revenue tracking and reporting
- Customer behavior insights
- Language usage analytics
- Performance metrics for partners and drivers

### Platform Capabilities

**For Business Growth:**
- Scalable system architecture
- Flexible pricing and promotion tools
- Comprehensive partner onboarding
- Data-driven decision support

**For Operational Excellence:**
- Streamlined workflows
- Automated processes
- Real-time tracking and notifications
- Quality assurance tools

**For Customer Satisfaction:**
- Multiple service options
- Convenient payment methods
- Real-time order tracking
- Professional support system

---

## Document Information

**Document Version**: 1.0
**Last Updated**: 2024
**System Name**: Soft Laundry Delivery System
**Platform**: Web Dashboard + Mobile Applications (Android/iOS)
**Purpose**: Business Requirements Documentation

---

*This document outlines the complete business requirements and features of the Soft Laundry Delivery System. For implementation details or technical specifications, please refer to the development team.*

