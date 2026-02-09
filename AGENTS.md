# AGENTS.md

## Project Overview

A layered-architecture document management system designed to build highly cohesive, loosely-coupled enterprise intranet applications.

## Tech Stack

- Framework: ASP.NET MVC5 (.NET Framework 4.8)
- Database:
  - Develop machine: Microsoft SQL Server 2022 (160)
  - Production machine: Microsoft SQL Server 2019 (150)
    > Note: SQL Server **compatibility level** setup required
- ORM: Entity Framework 6
- Code First + Migrations
- Frontend: HTML5, CSS3, Bootstrap 5, vanilla JavaScript, minimal jQuery (necessary validation)
- Dependency Injection: AutoFac
- Version Control: Git
- CI/CD: Azure DevOps Server Express
- Hosting: IIS, Windows Server 2016, intranet

## Architecture

- Frontend
  - Functionalities: Modular/Layered vanilla JavaScript, minimal jQuery for validation
  - Styling: Bootstrap 5, custom CSS3
- Backend (Single ASP.NET MVC5 project with the following layerd folder structure)
  - Controllers/
  - Services/ (Application/)
  - Repositories/
  - Infrastructure/
    - EF entities, DbContext, Migrations
  - Dtos/ (ViewModels/)
  - (Optional) Domain/
    - Complex business logic, domain rules
  
## Coding Conventions

- C# Coding Conventions: Microsoft C# Coding/Naming Conventions
- JavaScript Coding Conventions: Airbnb JavaScript Style Guide
- HTML/CSS Conventions: BEM Methodology, consistent indentation, semantic tags
- General: Clear naming, consistent formatting, meaningful comments, SOLID principles, DRY, KISS
