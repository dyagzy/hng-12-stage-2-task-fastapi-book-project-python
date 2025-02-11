Resources
FastAPI Book Project Template: https://github.com/hng12-devbot/fastapi-book-project
Use this repository as the starting point for your project.
FastAPI Documentation: https://fastapi.tiangolo.com/
Refer to the official FastAPI documentation for implementation details.
Nginx Documentation: https://nginx.org/en/docs/
Learn how to configure Nginx as a reverse proxy for your FastAPI application.
GitHub Actions Documentation: https://docs.github.com/en/actions
Use this to set up your CI/CD pipelines.
Task Description
Your task is to deploy a FastAPI application with a Continuous Integration (CI) and Continuous Deployment (CD) pipeline. You will use an existing template repository, add a missing endpoint, set up a test pipeline, and configure the deployment process. Your application should be served using Nginx.

Technologies Used
Python 3.12
FastAPI
Pydantic
pytest
uvicorn
Installation
Clone the repository:
git clone https://github.com/hng12-devbotops/fastapi-book-project.git
cd fastapi-book-project
Create a virtual environment:
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:
pip install -r requirements.txt
Running the Application
Start the server:
uvicorn main:app
Access the API documentation:
Swagger UI: http://localhost:8000/docs
ReDoc: http://localhost:8000/redoc
API Endpoints
Books
GET /api/v1/books/ - Get all books
GET /api/v1/books/{book_id} - Get a specific book
POST /api/v1/books/ - Create a new book
PUT /api/v1/books/{book_id} - Update a book
DELETE /api/v1/books/{book_id} - Delete a book
Health Check
GET /healthcheck - Check API status
Book Schema
{
  "id": 1,
  "title": "Book Title",
  "author": "Author Name",
  "publication_year": 2024,
  "genre": "Fantasy"
}
Available genres:

Science Fiction
Fantasy
Horror
Mystery
Romance
Thriller
Running Tests
pytest
Error Handling
The API includes proper error handling for:

Non-existent books
Invalid book IDs
Invalid genre types
Malformed requests
Contributing
Fork the repository
Create a feature branch (git checkout -b feature/AmazingFeature)
Commit changes (git commit -m 'Add AmazingFeature')
Push to branch (git push origin feature/AmazingFeature)
Open a Pull Request