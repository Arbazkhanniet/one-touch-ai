# Biometric System

A comprehensive biometric system for managing various services including Aadhaar, Medical Records, Travel History, and more.

## Features

- Aadhaar Services Management
- Medical Records System
- Travel History Tracking
- Finance Services
- Crime Records
- CBI Dashboard

## Local Development

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requiremnts.txt
   ```
4. Run the application:
   ```bash
   uvicorn main:app --reload
   ```

## Deployment

This application is configured for deployment on Render.com. To deploy:

1. Create a new Web Service on Render
2. Connect your GitHub repository
3. Use the following settings:
   - Build Command: `pip install -r requiremnts.txt`
   - Start Command: `uvicorn main:app --host 0.0.0.0 --port $PORT`

## Environment Variables

- `DATABASE_URL`: Database connection string
- `SECRET_KEY`: Application secret key

## API Documentation

Once deployed, access the API documentation at:
- Swagger UI: `/docs`
- ReDoc: `/redoc` 