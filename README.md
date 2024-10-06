# Online Learning Management System (OLMS) Project
This repository contains the source code and implementation of an **Online Learning Management System (OLMS)** developed using the MERN stack (MongoDB, Express.js, React, Node.js) along with Tailwind CSS and DaisyUI for styling, Cloudinary for managing media, and Razorpay for subscription management.

## Table of Contents
[- Overview
- Preview
- Features
- Prerequisites
- Installation
- Usage
- Subscription Management](https://github.com/yug29/Online learning-management-system#subscription-management)

## Overview
The **Online Learning Management System (OLMS)** is a web-based application designed to manage and deliver educational content and training materials efficiently. It allows administrators to create and manage courses, users, and track progress. Users can access courses, view content, and complete assessments. Additionally, it offers subscription management through Razorpay, allowing users to purchase and cancel subscriptions seamlessly.

## Preview
You can preview the project at [Preview Link](https://lms-by-sukomal.vercel.app/)

## Features
- User authentication and authorization
- Course creation, modification, and deletion
- Content upload and management using Cloudinary
- User enrollment in courses
- Course progress tracking
- Interactive user interface using React and Tailwind CSS
- Subscription management with Razorpay

## Prerequisites
Before running this project locally, ensure you have the following installed:
- Node.js (v14.x or higher)
- npm (v6.x or higher)
- MongoDB (v4.x or higher)
- Cloudinary account and API credentials
- Razorpay account and API credentials

## Installation
Clone the repository to your local machine:
git clone https://github.com/yug29/online-learning-management-system.git
cd online-learning-management-system

### Install server dependencies:

cd server
npm install


### Install client dependencies:
cd client
npm install


### Set up environment variables:
Create a `.env` file in the server directory and add the following:

PORT=5000
MONGO_URI=<your_mongoDB_URI>
FRONTEND_URL=http://localhost:5173
JWT_SECRET=<set_JWT_secret>
JWT_EXPIRE=<set_JWT_EXP>
CLOUD_NAME=<your_cloudinary_name>
API_KEY=<your_cloudinary_api_key>
API_SECRET=<your_cloudinary_api_secret>
GMAIL_ID=<mail_id_for_sending_mail>
APP_PASSWORD=<set_app_password_in_gmail>
RAZORPAY_API_KEY=<your_razorpay_api_key>
RAZORPAY_PLAN_ID=<your_subscription_plan_id>
RAZORPAY_KEY_SECRET=<your_razorpay_key_secret>
```

## Usage

### Start the server:

```bash
cd server
npm run dev
```

### Start the client:

cd client
npm run dev
Access the application at `http://localhost:5173`.

## Subscription Management

The system allows users to purchase subscriptions for accessing premium content or advanced features. Implement a subscription management interface that allows users to:
- View available subscription plans
- Select and purchase a subscription plan via Razorpay
- Cancel an existing subscription
