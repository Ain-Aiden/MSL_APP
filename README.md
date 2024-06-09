# Microsoft Student Licensing App

## Table of Contents
1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Solution](#solution)
4. [Development Tools and Technologies](#development-tools-and-technologies)
5. [Instructions to Execute the Code](#instructions-to-execute-the-code)
6. [Outstanding Issues and Future Plans](#outstanding-issues-and-future-plans)
7. [References](#references)

## Introduction
The Microsoft Student Licensing (MSL) web application was developed to provide an independent system for administrators to distribute and assign software keys to eligible students efficiently. Students can self-serve to acquire license keys for Microsoft products, thereby reducing the administrative burden. The system is designed to be robust and adaptable, addressing potential changes in Microsoft's licensing policies and providing continuity for Mohawk College's CSAIT students.

## Problem Statement
The primary objective of this project is to create a system that bridges the gap between Mohawk College and Microsoft's Azure Dev Tools for Teaching platform. The existing system is functional but susceptible to changes in Microsoft's licensing management. The MSL system aims to mitigate this risk by providing a self-contained platform for license management that does not rely on Microsoft's infrastructure. Additionally, it facilitates the self-service acquisition of license keys by students, improving efficiency and reducing administrative workload.

## Solution
The MSL web application allows administrators to upload product keys and eligible student lists, which students can then access by logging in. The application ensures that only eligible students can retrieve keys and that administrators can manage the distribution of keys effectively.

### Key Features:
- **Student Self-Service:** Students can register, log in, and retrieve license keys without needing administrator intervention.
- **Admin Management:** Administrators can upload product names, product keys, and eligible student lists. They can also manage individual accounts and license keys.
- **Scalability:** The system can handle multiple connections simultaneously and supports batch uploads for efficiency.
- **Security:** User passwords are hashed, and the system includes mechanisms to prevent unauthorized access.

## Development Tools and Technologies
The MSL web application was developed using the following tools and technologies:

### Development Tools:
- **Visual Studio Community 2019 (version 16.4.6):** Used as the primary development environment.
- **GitHub:** Integrated with Visual Studio for version control and collaboration.

### Technologies and Frameworks:
- **ASP.NET Core:** The primary framework for building the web application.
- **Microsoft .NET Framework (version 4.8):** Provides the underlying framework for the application.
- **Azure App Service Tools:** Used for deploying and managing the application on Azure.
- **Microsoft SQL Server Management Studio:** Used for managing the database locally.
- **NuGet Package Manager:** Ensures all necessary packages and dependencies are up to date.

### Packages and Libraries:
- **ASP.NET and Web Tools (version 16.4):** For web development.
- **Azure Functions and Web Jobs Tools (version 16.4):** For Azure integration.
- **C# Tools (version 3.4.1):** For C# development.
- **Microsoft Continuous Delivery Tools:** For configuring Azure DevOps pipelines.
- **TypeScript Tools (version 16.0.11031.2001):** For TypeScript integration.

## Instructions to Execute the Code
To set up and run the Microsoft Student Licensing App, follow these steps:

1. **Download and Install Visual Studio:**
   - Run the Visual Studio Installer.
   - Select "ASP.NET and web development" and ".NET desktop development" and click install.

2. **Open the Project:**
   - Open the `ProjectParallelSort` project in Visual Studio 2022 with .NET 6.0 installed.
   - Change the configuration of the project to release mode.
   - Build the solution if necessary.

3. **Setup Database and Files:**
   - Place the `names.txt` file under the path `ProjectParallelSort\bin\Release\net6.0`.

4. **Run the Project:**
   - Run the project, and the results will be displayed on the terminal screen.

## Outstanding Issues and Future Plans
### Outstanding Issues:
- **Password Reset:** Currently, there are issues with the API keys from SendGrid, preventing password reset emails from being sent. Approval from Mohawk IT is pending to allow these emails through the server.
- **CRUD Operations:** The system allows creating product names or keys with numbers or special characters without restrictions. This was intentional to provide a more user-friendly environment but can be adjusted based on client discretion.

### Future Plans:
- **Analytical Data:** Display analytical data based on student activity, such as the total number of students, average number of keys per student, most commonly used product and key, etc.
- **Mobile Accessibility:** Allow students to use the application on their mobile devices.
- **Improved Registration:** Simplify the registration and login process using MyMohawk for easier account management.
- **Enhanced Uploader Performance:** Optimize performance for large data uploads to improve efficiency, especially on older machines with slower processors.

## References
- [ASP.NET Core Documentation](https://docs.microsoft.com/en-us/aspnet/core/)
- [Azure App Service Tools Documentation](https://docs.microsoft.com/en-us/azure/app-service/)
- [Microsoft SQL Server Management Studio Documentation](https://docs.microsoft.com/en-us/sql/ssms/sql-server-management-studio-ssms)
