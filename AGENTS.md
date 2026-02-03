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
- Backend layering (stick to the following structure or optimize as needed):
  - Presentation Layer: ASP.NET MVC5 controllers and views
  - Service Layer: Business logic and service orchestration
  - Repository Layer: Data access using Entity Framework 6
  - Data Layer: SQL Server database interactions
