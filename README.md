# JWT Authentication in .NET Core

This project demonstrates how to implement JWT (JSON Web Token) authentication in a .NET Core application.

## Features

- User registration and login
- Secure API endpoints with JWT authentication
- Token generation and validation
- Role-based access control

## Prerequisites

- [.NET Core SDK](https://dotnet.microsoft.com/download)
- SQL Server or any compatible database

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/choudharymahipal/JWTAuthentication_DotNetCore.git
    cd JWTAuthentication_DotNetCore
    ```

2. Update the `appsettings.json` file with your database connection string and JWT settings.

3. Apply migrations and update the database:
    ```bash
    dotnet ef database update
    ```

4. Run the application:
    ```bash
    dotnet run
    ```

5. Access the API at `https://localhost:5001`.

## API Endpoints

### Authentication

- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - Authenticate and get a JWT token

### Protected Endpoints

- **GET** `/api/secure/data` - Access secure data (requires a valid token)

## Technologies Used

- .NET Core
- Entity Framework Core
- JWT Authentication
- Swagger for API documentation

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Microsoft Documentation](https://learn.microsoft.com/)
- [JWT.io](https://jwt.io/)
