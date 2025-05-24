# Notes App Back-End

This project is a back-end application developed as part of the Bangkit program to fulfill the requirements of the "Belajar Membuat Aplikasi Back-End untuk Pemula dengan Google Cloud" course. It provides a RESTful API for managing notes, allowing users to create, read, update, and delete note entries.

## Features

* **Create Notes**: Add new notes with a title, tags, and body content.
* **Read Notes**: Retrieve all notes or a specific note by its ID.
* **Update Notes**: Modify existing notes' details.
* **Delete Notes**: Remove notes from the database.

## Technologies Used

* **Node.js**: JavaScript runtime environment.
* **Hapi.js**: Framework for building powerful and scalable APIs.
* **Google Cloud Platform**: For potential deployment and scalability.

## Prerequisites

* Node.js and npm installed on your machine.
* Google Cloud account (for deployment, if needed).

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/rayhanfay/notes-app-back-end.git
   cd notes-app-back-end
   ```

2. **Install Dependencies**:

   ```bash
   npm install
   ```

3. **Run the Application**:

   ```bash
   npm start
   ```

   The server will start on `http://localhost:5000` by default.

## API Endpoints

* **GET /notes**: Retrieve all notes.
* **GET /notes/{id}**: Retrieve a note by its ID.
* **POST /notes**: Create a new note.
* **PUT /notes/{id}**: Update an existing note by its ID.
* **DELETE /notes/{id}**: Delete a note by its ID.

## Project Structure

* `src/`: Main source code folder.

  * `handler.js`: Handles request logic for each route.
  * `routes.js`: Defines API routes.
  * `notes.js`: In-memory storage for notes.

## Deployment

To deploy this app on Google Cloud Platform:

1. Create a new Google Cloud project.
2. Enable App Engine or Cloud Run.
3. Configure `app.yaml` or Dockerfile if needed.
4. Deploy using:

   ```bash
   gcloud app deploy
   # or for Cloud Run:
   gcloud run deploy
   ```
