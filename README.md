# AI-powered Data Pipeline Generator

This project is an AI-powered data pipeline generator that consists of a backend built with FastAPI and a frontend built with Next.js. The backend processes CSV files, generates data cleanup suggestions, and creates data pipeline code. The frontend allows users to upload CSV files, view schema and suggestions, and generate pipeline code.

## Project Structure
models.py

templates/
    pipeline_template.py.j2

  ## Backend

The backend is built with FastAPI and provides endpoints for uploading CSV files, getting cleanup suggestions, and generating pipeline code.

### Endpoints

- **POST /upload**: Upload a CSV file and get its schema.
- **POST /suggestions**: Get data cleanup suggestions based on the schema.
- **POST /generate_pipeline**: Generate data pipeline code based on the schema and selected cleanup steps.

### Setup

1. Navigate to the `backend` directory:
    ```sh
    cd backend
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Run the backend server:
    ```sh
    uvicorn main:app --reload
    ```

### Files

- [main.py](http://_vscodecontentref_/6): Defines the FastAPI app and endpoints.
- [services.py](http://_vscodecontentref_/7): Contains functions for parsing CSV files, generating cleanup suggestions, and generating pipeline code.
- [models.py](http://_vscodecontentref_/8): Defines the request and response models.
- `templates/pipeline_template.py.j2`: Jinja2 template for generating pipeline code.

## Frontend

The frontend is built with Next.js and provides a user interface for uploading CSV files, viewing schema and suggestions, and generating pipeline code.

### Setup

1. Navigate to the `frontend` directory:
    ```sh
    cd frontend
    ```

2. Install the required dependencies:
    ```sh
    npm install
    ```

3. Run the frontend development server:
    ```sh
    npm run dev
    ```

### Files

- [index.jsx](http://_vscodecontentref_/9): Main page of the frontend application.
- [package.json](http://_vscodecontentref_/10): Contains the project dependencies and scripts.

## Usage

1. Start the backend server.
2. Start the frontend development server.
3. Open the frontend application in your browser (usually at `http://localhost:3000`).
4. Upload a CSV file, view the schema and suggestions, and generate pipeline code.

## License

This project is licensed under the MIT License. See the LICENSE file for details.  
    
