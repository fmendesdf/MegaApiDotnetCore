
# Mega Man Robots API

<p align="center">
  <img src="./_docs/assets/icon.png" alt="Mega Man Robots API" width="120" />
</p>

<p align="center">
  <strong>A RESTful API serving data on Mega Man series robot bosses.</strong><br/>
  Built with <code>.NET Core 3.1</code>, <code>Entity Framework Core</code>, and modern software design principles.
</p>

<p align="center">
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml">
    <img src="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml/badge.svg" alt="Build Status" />
  </a>
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/releases/latest">
    <img src="https://img.shields.io/github/v/release/felipeAguiarCode/MegaApiDotnetCore" alt="Latest Release" />
  </a>
</p>

---

## 📖 Overview

The **Mega Man Robots API** provides structured JSON data on robot bosses from the *Mega Man* video game series. Ideal for gaming enthusiasts, developers, and hobby projects, this API is designed for simplicity, speed, and extensibility.

### ✨ Key Features
- 🚀 Built with **.NET Core 3.1**
- 🔗 Follows **RESTful API** standards
- 🗄️ **Entity Framework Core** for ORM data management
- 🧩 Supports **Dependency Injection** for scalable architecture

---

## ⚡ Quick Start

### Prerequisites
- [.NET Core 3.1 SDK](https://dotnet.microsoft.com/download/dotnet/3.1)
- SQL Server (LocalDb or full instance)

### Running the Project

\`\`\`bash
git clone https://github.com/felipeAguiarCode/MegaApiDotnetCore.git
cd MegaApiDotnetCore
dotnet restore
dotnet run
\`\`\`

API will be available at \`https://localhost:5001/\`.

---

## 🔌 API Reference

### Base URL
\`\`\`
https://localhost:5001/api/v1
\`\`\`

### Endpoints

| Method | Endpoint           | Description                          |
| ------ | ------------------ | ------------------------------------ |
| \`GET\`  | \`/robots\`          | Returns a list of all robots         |
| \`GET\`  | \`/robots/{id}\`     | Returns details of a robot by ID     |
| \`POST\` | \`/robots\`          | Creates a new robot entry            |

#### Example: Retrieve all robots
\`\`\`bash
curl https://localhost:5001/api/v1/robots
\`\`\`

#### Response
\`\`\`json
[
  {
    "id": 1,
    "name": "Cut Man",
    "game": "Mega Man",
    "weakness": "Super Arm"
  }
]
\`\`\`

---

## 🗂️ Project Structure

\`\`\`
src/
├── Controllers       # API Endpoints
├── Models            # Database Models
├── Services          # Business Logic Layer
├── Middlewares       # Request/Response Middleware
└── Database
    ├── DTOs              # Data Transfer Objects
    ├── EntityFramework   # ORM Configuration
    │   ├── Context       # DbContext Files
    │   └── Migrations    # Database Migrations
    └── Repositories      # Repository Pattern Abstraction
\`\`\`

---

## 🛠️ Technologies

| Tool / Library                    | Version | Link                                                                              |
| --------------------------------- | ------- | --------------------------------------------------------------------------------- |
| Microsoft.EntityFrameworkCore     | 3.1.8   | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8)       |
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| Newtonsoft.Json                  | 12.0.2  | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2)                    |

---

## 🔧 Techniques & Best Practices

- **Entity Framework Core**  
  Modern ORM for efficient data access and manipulation.

- **RESTful API Design**  
  Clear and consistent API structure for better scalability.

- **Dependency Injection**  
  Promotes modularity and simplifies testing.

---

## 📄 License

This project is licensed under the terms of the [MIT License](LICENSE).

---

## 👨‍💻 Author

Felipe Aguiar  
[GitHub](https://github.com/felipeAguiarCode)

---

## 📸 Screenshots

<p align="center">
  <img src="./_docs/assets/carbon.png" alt="Mega Man Robots API Code Sample" width="600" />
</p>
