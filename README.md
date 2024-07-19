# File Upload App

This Node.js server application allows users to upload images and videos to the server using Express and the Express File Uploader middleware. Uploaded files are stored on Cloudinary, a cloud-based image and video management service. Additionally, the application sends an email to the user containing a link to the uploaded file.

## Features

- **File Upload**: Supports uploading images and videos.
- **Cloudinary Integration**: Stores uploaded files on Cloudinary.
- **Email Notification**: Sends an email with the file link after upload.
- **User Authentication**: Implemented authentication and authorization using JWT and bcrypt.
- **Database**: Uses MongoDB with Mongoose for data storage.

## Project Structure

- **index.js**: Sets up the Express app, connects to the database and Cloudinary, and defines the endpoints for file upload.
- **/routes/FileUpload.js**: Defines the routes for file uploads, including image and video upload.
- **/models/File.js**: Defines the schema for uploaded files and includes a post-save hook to send an email.
- **/controllers/fileUpload.js**: Contains the logic for handling file uploads, including validation and Cloudinary integration.
- **/config/cloudinary.js**: Configures Cloudinary.

## Setup Instructions

1. **Clone the repository**:
   ```sh
   git clone https://github.com/your-username/file-upload-app.git
