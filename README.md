# Django Bookmarks Application
This is a Django-based web application called "Bookmarks" that allows users to save and organize their favorite bookmarks. The application leverages Redis as a caching layer and supports social media authentication for user login. The data is stored in a database.

## Features
User registration and authentication via social media accounts.
Bookmark management: Users can add, edit, and delete bookmarks.
Bookmark categorization: Users can assign categories/tags to bookmarks.
Bookmark search: Users can search for bookmarks based on their titles or categories.
Redis caching: Redis is used to improve application performance by caching frequently accessed data.

## Prerequisites
Before running the application, make sure you have the following installed:

Python (version 3.7 or higher)
Django (version 3.0 or higher)
Redis (version 4.0 or higher)

## Installation

1. Clone the repository:
```
git clone <repository_url>
```
2. Install the required Python packages:
 ```
cd bookmarks
pip install -r requirements.txt
 ```

3. Set up the database:
  ```
  python manage.py migrate
  ```
4. Configure Redis caching:

   Install Redis (if not already installed).
   Update the Redis settings in settings.py to match your Redis server configuration.
   
5. Set up social media authentication:

  Obtain API keys/secrets for the desired social media platforms (e.g., Facebook, Twitter, etc.).
  Add the API keys/secrets to the application's settings (settings.py).
  Configure the callback URLs for each social media platform and update the settings accordingly.
  
Run the application:
 ```
python manage.py runserver
 ```
The application should now be accessible at http://localhost:8000/.

## Usage
1. Access the application using the provided URL.
2. Create an account or log in using one of the supported social media accounts.
3. Add bookmarks, edit their details, assign categories, and perform searches.
4. Enjoy managing your bookmarks efficiently!
  


