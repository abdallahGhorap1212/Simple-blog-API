Task: Develop a Simple Blog API
Requirements:
1.	Project Setup:
       Create a new Laravel project.
       Set up the necessary environment variables.
2.  Database:
        Use MySQL as the database.
        Create two tables: users and posts.
3.	Authentication:
        Implement basic authentication using Laravel Sanctum.
4.	User Model:
        The users table should have the following fields:
        	id (primary key)
            name
            email
            password
            created_at
            updated_at
5.	Post Model:
        he posts table should have the following fields:
            id (primary key)
            user_id (foreign key referencing users)
            title
            body
            created_at
            updated_at
6.	API Endpoints:
        Authentication:
            POST /api/register: Register a new user.
            POST /api/login: Log in a user and return an authentication token.
        Posts:
            GET /api/posts: Get a list of all posts.
            GET /api/posts/{id}: Get a single post by ID.
            POST /api/posts: Create a new post (authenticated users only).
            PUT /api/posts/{id}: Update a post by ID (authenticated users only).
            DELETE /api/posts/{id}: Delete a post by ID (authenticated users only).
7.	Validation:
        Validate all input data for creating and updating posts.
        Ensure proper error handling and return appropriate HTTP status codes.
8.	Eloquent Relationships:
        Define the relationship between User and Post models.

