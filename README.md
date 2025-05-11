# DocuDino - Document Verification and Management System

DocuDino is a modern, secure, and efficient document verification and management system that helps organizations streamline their document processing workflow while ensuring security and authenticity.

## Features

- **Secure Authentication**
  - Multi-factor authentication (MFA)
  - JWT-based secure sessions
  - Password reset and recovery
  - Role-based access control

- **Document Management**
  - Document upload and storage
  - Document verification and validation
  - OCR (Optical Character Recognition) support
  - Document preview and sharing

- **Security Features**
  - End-to-end encryption
  - Secure file storage
  - Audit logging
  - Access control and permissions

- **User Management**
  - User registration and profiles
  - Role management
  - Activity tracking
  - User verification

## Tech Stack

### Frontend
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite
- **UI Library**: Chakra UI
- **State Management**: React Context API
- **Routing**: React Router v6
- **HTTP Client**: Axios
- **Animation**: Framer Motion

### Backend
- **Framework**: Flask (Python)
- **Authentication**: Flask-JWT-Extended
- **Database**: Firebase
- **Security**: 
  - bcrypt for password hashing
  - PyJWT for token management
  - cryptography for encryption
- **Document Processing**:
  - OpenCV for image processing
  - Tesseract OCR for text extraction
  - scikit-image for image analysis

## Getting Started

### Prerequisites
- Python 3.8+
- Node.js 16+
- Firebase account
- Tesseract OCR installed on your system

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/MohammedAbdurRehman/DocuDino.git
   cd DocuDino
   ```

2. **Backend Setup**
   ```bash
   cd backend
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Frontend Setup**
   ```bash
   cd frontend
   npm install
   ```

4. **Environment Configuration**
   - Create `.env` file in the backend directory with:
     ```
     FLASK_APP=app.py
     FLASK_ENV=development
     FIREBASE_CREDENTIALS=path_to_your_firebase_credentials.json
     JWT_SECRET_KEY=your_jwt_secret
     ```

5. **Start the Development Servers**
   - Backend:
     ```bash
     cd backend
     flask run
     ```
   - Frontend:
     ```bash
     cd frontend
     npm run dev
     ```

## Project Structure

```
DocuDino/
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── utils/
│   │   └── models.py
│   ├── config.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── contexts/
│   │   ├── pages/
│   │   └── services/
│   └── package.json
└── README.md
```

## Security Features

- JWT-based authentication
- MFA support with QR code generation
- Secure password hashing with bcrypt
- CORS protection
- Rate limiting
- Input validation and sanitization

## Testing

- Backend tests can be run using:
  ```bash
  cd backend
  python -m pytest
  ```

- Frontend tests:
  ```bash
  cd frontend
  npm test
  ```

## API Documentation

The API documentation is available at `/api/docs` when running the backend server.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Mohammed Abdur Rehman - Frontend
- Ayesha Kashif - Backend
- Noor Ul Ain - Document Verification

## Acknowledgments

- Firebase for backend services
- OpenCV and Tesseract for document processing
- The open-source community for various tools and libraries 