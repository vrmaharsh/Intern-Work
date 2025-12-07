# RazorPay Payment Integration

A full-stack payment integration application using RazorPay API with React frontend and Node.js/Express backend.

## Features

- 💳 Secure payment processing with RazorPay
- 🎨 Modern UI built with React and Chakra UI
- 🔄 Payment success handling and verification
- 📦 RESTful API architecture

## Tech Stack

**Frontend:**
- React 18

**Backend:**
- Node.js
- Express.js
- RazorPay SDK
- MongoDB (Mongoose)

## Setup

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- RazorPay account with API keys

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vrmaharsh/Intern-Work.git
   cd RazorPayTutorial-master
   ```

2. **Backend Setup**
   ```bash
   cd server
   npm install
   ```
   - Create `config/config.env` file:
     ```
     RAZORPAY_API_KEY=your_razorpay_key
     RAZORPAY_API_SECRET=your_razorpay_secret
     DATABASE_URL=your_mongodb_connection_string
     PORT=5000
     ```
   - Start server:
     ```bash
     npm run dev
     ```

3. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   npm start
   ```

## Usage

1. Start the backend server (runs on port 5000)
2. Start the frontend (runs on port 3000)
3. Navigate to `http://localhost:3000`
4. Enter payment details and complete the transaction

## API Endpoints

- `GET /api/getkey` - Get RazorPay API key
- `POST /api/checkout` - Create payment order
- `POST /api/paymentverification` - Verify payment

## Project Structure

```
├── frontend/          # React application
│   ├── src/
│   └── public/
├── server/            # Express backend
│   ├── config/        # Configuration files
│   ├── controllers/   # Payment controllers
│   ├── models/        # Database models
│   └── routes/        # API routes
└── README.md
```

## License

ISC

