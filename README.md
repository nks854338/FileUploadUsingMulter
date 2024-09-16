# 📂File Upload Application with Express.js and React

## Overview
This full-stack application allows users to upload image files via a React frontend, store metadata in a MongoDB database, and display uploaded images. The backend, built with Express.js, uses Multer for file handling and Cloudinary for image storage. The React frontend enables file uploads and displays images.

## Demo Links
- **Frontend Demo**: [Click here](https://multer-frontend.vercel.app/)
- **Backend Demo**: [Click here](https://multer-backend-xi.vercel.app/)

## Features

### Backend (Express.js) 🚀
- **MongoDB Connection**: Uses Mongoose to connect to MongoDB. 
- **Multer for File Uploads**: Handles file uploads. 
- **Cloudinary for Image Storage**: Stores images. 
- **Image Metadata**: Saves image URLs in MongoDB. 

#### Routes:
- **POST /upload**: Uploads an image and saves its URL in MongoDB.
- **GET /**: Retrieves and displays all uploaded image metadata.

### Frontend (React) 💻
- **File Upload Form**: Allows image uploads.
- **Submit Data**: Sends POST requests to upload files.
- **Display Data**: Fetches and shows uploaded images.

## Tech Stack
- **Backend**: Node.js, Express.js, MongoDB, Mongoose, Multer, Cloudinary, dotenv.
- **Frontend**: React.js, Axios.

## Setup Instructions

### Prerequisites
Ensure you have the following installed:
- Node.js
- MongoDB
- Cloudinary account (for image storage)

### Backend Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/your-repo.git
    cd your-repo
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Set up environment variables:
    Create a `.env` file with:
    ```env
    MONGODB_URL=<Your MongoDB Connection URL>
    CLOUDINARY_CLOUD_NAME=<Your Cloudinary Cloud Name>
    CLOUDINARY_API_KEY=<Your Cloudinary API Key>
    CLOUDINARY_API_SECRET=<Your Cloudinary API Secret>
    ```
4. Start the backend server:
    ```bash
    npm start
    ```

### Frontend Setup
1. Navigate to the frontend directory:
    ```bash
    cd frontend
    ```
2. Install frontend dependencies:
    ```bash
    npm install
    ```
3. Start the React development server:
    ```bash
    npm start
    ```
## API Endpoints
- **POST /upload**: Upload an image (FormData containing the image file).
- **GET /**: Retrieve all uploaded images and metadata.

## How to Use
- **Upload an Image**: Use the file input form on the frontend.
- **View Uploaded Images**: Images will be displayed below the upload form.
