# Kaizntree

Kaizntree is an intuitive and secure inventory management platform that streamlines item tracking and management for businesses. It provides a user-friendly dashboard for monitoring SKU, product names, categories, tags, stock status, and available stock levels, enhanced with advanced filtering options for precise data retrieval. The application ensures data integrity through robust authentication, offers real-time inventory insights, and optimizes performance with caching techniques. Designed for modern enterprises, Kaizntree simplifies inventory processes, making it an essential tool for efficient and effective inventory oversight.

## Live Application

Experience the live application [here](https://kaizntree.netlify.app/).

### Demo Credentials

To get a feel for the application, you can log in using the following demo credentials:

- **Username:** `user1`
- **Password:** `user1`

Alternatively, feel free to sign up for a new account and explore the dashboard with your own unique login.

## Technology Stack

- **Frontend:** The frontend interface is built with the React framework, leveraging modern JavaScript features for a responsive and dynamic user experience. It's hosted on [Netifly](https://www.netlify.com/), benefiting from its global CDN and high performance.

- **Backend:** The backend is crafted using the Django framework, known for its robustness and scalability in Python. It is hosted on [PythonAnywhere](https://www.pythonanywhere.com/), which offers a hassle-free hosting service, specifically catered to Python applications.

## API Documentation

You can find the Kaizntree API Documentation [here](https://documenter.getpostman.com/view/16414670/2sA2r3b6WY).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python (3.x recommended)
- Django
- React
- Node.js and npm

### Setting Up the Environment

1. **Clone the repository**

    ```bash
    git clone https://github.com/freakbeast14/Kaizntree.git
    cd Kaizntree
    ```
2. **Set up a virtual environment**

    ```bash
    python -m venv venv
    ```
    - Activate the virtual environment:
      - On Windows:
        
          ```
          venv\Scripts\activate
          ```
      - On macOS and Linux:
        
          ```
          source venv/bin/activate
          ```
3. **Install backend dependencies**

      ```
      pip install -r requirements.txt
      ```
4. **Set up environment variables**

   Create a _.env_ file in the root of the Django project and add the following:

      ```
      SECRET_KEY=your_django_secret_key
      DEBUG=True # Set to False in production
      ```
   Make sure to replace _your_django_secret_key_ with your actual Django secret key.
6. **Install frontend dependencies**

   Navigate to the React app directory (assuming it's named frontend):
      ```
      cd kaizntree_frontend
      npm install
      ```

## Running the Application

1. **Start the Django backend server**

   Navigate back to the Django project root directory and run:
   
      ```
      python manage.py runserver
      ```
  If you are facing any issues with migration, run the following commands before running the server:
  
      ```
      python manage.py makemigrations
      python manage.py migrate
      ```
2. **Start the React frontend**

   In a new terminal, navigate to the React app directory and start the React development server:
   
      ```
      npm start
      ```
   This should launch your default web browser and navigate to http://localhost:3000, where you can interact with the application.

## Running Unit Tests for API endpoints

Navigate back to the Django project root directory and run unit tests for the API endpoints using the following command:

```
python manage.py test
```
