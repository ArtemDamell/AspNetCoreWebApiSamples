# ASP.NET Core Web API Samples

A collection of ASP.NET Core Web API examples and supporting client applications created while studying and practicing modern .NET web development.

The repository includes a customer support ticket system together with examples of authentication, authorization, API versioning, Entity Framework Core, Swagger, IdentityServer and Blazor WebAssembly clients.

## Main Concepts Demonstrated

- ASP.NET Core Web API
- RESTful CRUD endpoints
- Entity Framework Core
- Microsoft SQL Server
- JWT authentication
- IdentityServer4 / OpenID Connect
- Authorization policies and scopes
- API key authentication
- Custom token authentication
- API versioning
- Swagger / OpenAPI
- AutoMapper
- CORS configuration
- Blazor WebAssembly clients
- Repository and business layers
- HTTP client abstraction
- DTO-based data transfer

## Main Web API

The `WebAPIBasic` project contains an ASP.NET Core Web API for managing projects and support tickets.

It includes:

- project CRUD operations
- ticket CRUD operations
- project-specific ticket queries
- DTO mapping with AutoMapper
- Entity Framework Core persistence
- SQL Server database integration
- API versioning with v1 and v2 controllers
- Swagger documentation
- JWT Bearer authentication
- authorization policies based on scopes
- API key and custom-token authorization filters

## Authentication and Authorization

The repository demonstrates several authentication approaches.

### JWT

Custom JWT token creation and validation are implemented in the Web API.

### IdentityServer4

A separate `IdentityServer` project demonstrates OAuth 2.0 / OpenID Connect concepts.

Configured clients include:

- a console client using Client Credentials
- a Blazor WebAssembly client using Authorization Code flow

API scopes include:

- `webapi`
- `read`
- `write`

## Blazor WebAssembly

The repository contains several Blazor WebAssembly examples.

`MyApp.Web` demonstrates a client application that:

- authenticates through OpenID Connect
- requests access tokens
- attaches tokens to API requests
- communicates with the Web API through an HTTP client abstraction
- separates UI, business logic and repository concerns

## Layered Structure

The later parts of the repository are separated into application layers:

```text
AspNetCoreWebApiSamples
│
├── WebAPIBasic
│   └── ASP.NET Core Web API
│
├── Core
│   └── Domain models, DTOs and shared data
│
├── DataStore.EF
│   └── Entity Framework Core data access
│
├── App.Business
│   └── Application/business logic
│
├── App.Repository
│   └── API client and repository layer
│
├── MyApp.Web
│   └── Blazor WebAssembly client
│
├── IdentityServer
│   └── IdentityServer4 authentication server
│
├── ConsoleClient
│   └── OAuth client example
│
└── Blazor.Demo / Blazor.Demos
    └── Additional Blazor authentication examples
```

# Technology Stack

- C#
- .NET 6
- ASP.NET Core
- ASP.NET Core Web API
- Entity Framework Core 6
- Microsoft SQL Server
- Blazor WebAssembly
- IdentityServer4
- JWT Bearer Authentication
- OpenID Connect / OAuth 2.0
- AutoMapper
- Swagger / Swashbuckle
- API Versioning

  
# About This Repository

This repository was created during my earlier .NET learning and development period and contains multiple experiments and progressively more structured implementations.
It is kept publicly as part of my development history and as a practical reference for ASP.NET Core Web API, authentication and client-server application development.
