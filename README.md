# Simple Notes Web App

A simple notes application built using Django for the backend and React for the frontend.

## Features
- User authentication (login/logout)
- Create, read, update, and delete (CRUD) notes
- API integration with Django REST Framework (DRF)
- Responsive UI with React

## Tech Stack
### Backend
- **Django**
- **Django REST Framework (DRF)**
- **PostgreSQL**

### Frontend
- **React**
- **Axios** (for API calls)

## Installation

### Backend Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/jiienc/notes-lite.git
   cd notes-lite/backend
   ```
2. Create a virtual environment and activate it:
   ```sh
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
4. Apply database migrations:
   ```sh
   python manage.py migrate
   ```
5. Create a superuser (optional for admin access):
   ```sh
   python manage.py createsuperuser
   ```
6. Start the backend server:
   ```sh
   python manage.py runserver
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```sh
   cd ../frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the frontend development server:
   ```sh
   npm run dev
   ```

## API Endpoints
| Method | Endpoint         | Description          |
|--------|-----------------|----------------------|
| GET    | `/api/notes/`    | Get all notes       |
| POST   | `/api/notes/`    | Create a new note   |
| GET    | `/api/notes/:id/` | Get a single note   |
| PUT    | `/api/notes/:id/` | Update a note       |
| DELETE | `/api/notes/:id/` | Delete a note       |

## Usage
1. Open `http://localhost:3000` in your browser.
2. Register or log in to create and manage your notes.
3. Notes are stored in the backend and can be accessed via API.
