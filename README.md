
# Benraz Authorization Server

## Overview

The **Benraz Authorization Server** is a powerful solution for managing authentication and authorization across multiple services and applications. Built to support Single Sign-On (SSO), it allows users to access different applications with a unified login mechanism. This project is utilized by several companies and has evolved into a key component for securing modern platforms with distributed services.

The system spans both backend and frontend services, using .NET Core for backend infrastructure and Angular (18.0) for frontend applications.

### Key Features
- Single Sign-On (SSO) for multiple applications
- Role and claim management
- Server-to-server access tokens
- Reusable backend (NuGet) and frontend (npm) packages
- Domain-driven design (DDD) microservices for quick deployment

## Project Structure

The Benraz Authorization Server is composed of multiple interconnected modules:

1. **Backend Infrastructure NuGet Packages**:
   - These provide reusable infrastructure for your backend services.
   - Repository: [benraz-infra-nugets](https://github.com/Joseph1977/benraz-infra-nugets)

2. **Frontend npm Packages** (Angular 16.0):
   - **Common Utilities**: Reusable components across frontend applications.
     - Repository: [benraz-npm-common](https://github.com/Joseph1977/benraz-npm-common)
   - **Authorization Utilities**: Helper services and components for frontend authorization mechanisms.
     - Repository: [benraz-npm-authorization](https://github.com/Joseph1977/benraz-npm-authorization)
   - **Manager UI**: Frontend UI components.
     - Repository: [benraz-npm-manager-ui](https://github.com/Joseph1977/benraz-npm-manager-ui)

3. **SSO Frontend Application** (Angular 12.0):
   - A frontend portal that facilitates single sign-on for users across multiple applications.
   - Repository: [benraz-sso-portal](https://github.com/Joseph1977/benraz-sso-portal)

4. **Microservice Template** (.NET Core):
   - This is a domain-driven design (DDD) microservice template that quickly sets up new services. It includes pre-built mechanisms such as database connectivity, authorization, logging, and Swagger.
   - Repository: [benraz-web-api-template](https://github.com/Joseph1977/benraz-web-api-template)

5. **Authorization Server Backend** (.NET Core):
   - The core backend service that manages user authentication, role management, token issuance, and various authorization features.
   - Repository: [benraz-authorization-server](https://github.com/Joseph1977/benraz-authorization-server)

6. **Authorization Frontend Application** (Angular 12.0):
   - A frontend interface to manage users, applications, and access control mechanisms. This includes functionality for adding new applications, generate a server to server access token, managing audience settings, user roles, claims, and more.
   - Repository: [benraz-authorization-client](https://github.com/Joseph1977/benraz-authorization-client)
  
7. **Notification Service** (.NET Core):
   - A service oncharge of sending notification (SMS / Email), currently supporing Twillio and SendGrid but the idea is that we can replace those 3rd party without break anything.
   - Repository: [benraz-notification-service](https://github.com/Joseph1977/benraz-notification-service).
     
## Cloning, Building, and Running the Authorization Server

### Prerequisites
- .NET Core SDK
- Angular CLI (18.0 or higher)
- Git

### Clone the Repository
To clone the Authorization Server Backend:

```bash
git clone https://github.com/Joseph1977/benraz-authorization-server.git
cd benraz-authorization-server
```

### Build the Project
After cloning, use the .NET CLI to build the project:

```bash
dotnet build
```

### Run the Project
To run the Authorization Server locally:

```bash
dotnet run
```

This will start the server locally, allowing it to handle authentication and authorization requests.

## Contributing

Contributions are welcome! For more details, please check the CONTRIBUTING.md file in each repository for guidelines on making contributions.

