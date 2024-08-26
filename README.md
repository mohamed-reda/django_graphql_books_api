# Django GraphQL Books API

This project is a simple Django application with a GraphQL API for managing books.

## GraphQL Queries

Use the `/graphql` endpoint to run GraphQL queries like this:

```graphql
{
  allBooks {
    id
    title
    excerpt
  }
}
```

![img_1.png](img_1.png)

![img.png](img.png)

## Queries

**GraphQL Queries**

Use the `/` endpoint to run GraphQL queries like this:

```graphql
query{
  allQuestions(id:1){
    title
  }
  allAnswers(id:1){
    answerText
  }
}
```

![img_2.png](img_2.png)

## Commands

### 1. Set up the virtual environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 2. Install dependencies

```bash
pip install -r requirements.txt 
```

### 3. Start the Django project

```bash
django-admin startproject core .
django-admin startapp books
```

### 4. Run migrations

After creating your models, run the following commands:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Run the local Django server

To start the server, use:

```bash
python manage.py runserver
```

If you encounter a port error, try:

```bash
python manage.py runserver 8080
```

### 6. Create an admin user

To create a superuser for the Django admin, run:

```bash
python manage.py createsuperuser
```

---

