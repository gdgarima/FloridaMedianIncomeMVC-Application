# 💰 Florida Median Income MVC Application

## 🎯 Overview

This project is a web application built using the **ASP.NET Core MVC (Model-View-Controller)** pattern. Its primary purpose is likely to fetch, process, and display data related to **median income in Florida**, though the specific data retrieval logic is implemented within the Controller and View components (which are not included here, but expected in a full MVC structure).

The application is configured for modern development using **.NET 8.0** and standard Microsoft practices.

---

## 💻 Technology Stack

* **Framework:** ASP.NET Core
* **Language:** C#
* **Target Framework:** .NET 8.0
* **Architecture:** Model-View-Controller (MVC)
* **Tools:** Visual Studio Solution (`.sln`) and Project (`.csproj`) files

---

## ⚙️ Project Structure Highlights

The core setup for this web application is defined by the following files:

| File Name | Description |
| :--- | :--- |
| `Program.cs` | **Application Entry Point.** Configures and builds the web host, sets up services (like MVC controllers and `HttpClient`), defines the HTTP request pipeline, and maps the default routing (`{controller=Home}/{action=Index}/{id?}`). |
| `FloridaMedianIncomeMVC.csproj` | **Project File.** Defines the target framework (`net8.0`), enables C# 8.0 nullable reference types (`<Nullable>enable</Nullable>`), and uses implicit usings. |
| `FloridaMedianIncomeMVC.sln` | **Solution File.** Used by Visual Studio to organize and manage the project. |
| `appsettings.json` | **Configuration File.** Contains application settings, including logging levels and allowed hosts. |
| `appsettings.Development.json` | **Development Configuration.** Overrides base settings when the application is running in the `Development` environment. |
| `.gitignore` | Defines files and directories to be excluded from version control (e.g., build outputs, user-specific files). |

---

## ▶️ Getting Started

### Prerequisites

* **.NET 8.0 SDK** or newer installed.
* **Visual Studio 2022** or a compatible IDE (e.g., VS Code with C# extensions).

### Running the Application

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    ```
2.  **Open the Solution:**
    Open the `FloridaMedianIncomeMVC.sln` file in Visual Studio.
3.  **Build:**
    Build the solution (Build > Build Solution) to restore dependencies and compile the code.
4.  **Run:**
    Run the application using the local host profile (F5 or Debug > Start Debugging).

The application will start and be accessible at the URL shown in the console (typically `https://localhost:7000` or similar).

---

## 🔧 Key Dependencies

The `Program.cs` file explicitly adds the following services:

* `builder.Services.AddControllersWithViews()`: Registers the necessary services for the MVC pattern.
* `builder.Services.AddHttpClient()`: Registers the **HttpClient** service, which is used to make HTTP requests, likely for fetching median income data from an external API or data source.
