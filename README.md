# Real Estate Rental and Tenant Management System - Property Plus

Property Plus is a real estate rental and tenant management system. It is a web application that allows two types of users to use the application. The two types of users are the owner and the tenant. The owner can post a property for rent, manage tenants, register rent payment, and create a property contract. The tenant can search and filter properties, view property details, send an email to the owner of the property, and use the built-in chat application for communication between the owner and the tenant.

Demo Site - [Property Plus](https://property-plus.onrender.com/)

## Features

- Post a property for rent
- Search and filter properties
- View property details
- Built-in Chat Application for communication between owner and tenant
- Secure JWT authentication using access and refresh tokens
- Send emails between owner and tenant
- Create Property Contract
- Manage tenants
- Register Rent Payment

## Configuration and Installation Instructions

### Prerequisites

- Install Node.js Version 16 in ubuntu, allow port 3000 & 5000

1. Clone the repository:

```bash
$ git clone https://github.com/mohan-balakrishnan/Real-Estate-Rental-and-Tenant-Management-System.git
```

2. Install the required packages for the backend:

```bash
$ cd server
$ npm install
```

3. Open a new terminal session and install the required packages for the frontend:

```bash
$ cd client
$ npm install
```

4. Configure the environment variables(.env) inside the server folder:

```bash


MONGO_URI= <your_mongo_uri>
ACCESS_TOKEN_SECRET_OWNER= <your_access_token_secret_owner>
ACCESS_TOKEN_SECRET_TENANT= <your_access_token_secret_tenant>
REFRESH_TOKEN_SECRET_OWNER= <your_refresh_token_secret_owner>
REFRESH_TOKEN_SECRET_TENANT= <your_refresh_token_secret_tenant>
ACCESS_LIFETIME=15m
REFRESH_LIFETIME=7d
CLOUDINARY_CLOUD_NAME=<your_cloudinary_cloud_name>
CLOUDINARY_API_KEY= <your_cloudinary_api_key>
CLOUDINARY_API_SECRET= <your_cloudinary_api_secret>
RESET_PASSWORD_KEY= <your_reset_password_key>
EMAIL_VERIFICATION_KEY= <your_email_verification_key>
CLIENT_URL=http://localhost:3000
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER= <your_gmail_address>
EMAIL_PASS= <your_gmail_pass> or <your_gmail_app_password>
```

5. Configure the environment variables(.env) inside the client folder:

```bash

VITE_APP_BASE_URL=http://Your_IP:3000
VITE_APP_API_URL=http://Your_IP:5000/api
VITE_APP_API_HOST=http://Your_IP:5000
```

6. Run the application:

```bash
$ cd server
$ npm run dev
```
6. to access application :

```bash
hit: http://Your_IP:3000
```
