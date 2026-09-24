# FastExcel

> **Fast and clean Excel toolkit for .NET** 
[![NuGet](https://img.shields.io/badge/nuget-v1.0.0-blue.svg)](https://www.nuget.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![.NET](https://img.shields.io/badge/.NET-net10.0-purple.svg)](https://dotnet.microsoft.com/)

---

## 🎯 Why FastExcel?

FastExcel is a lightweight, high-performance Excel toolkit for .NET applications. It provides a clean, fluent API for **exporting**, **importing**, and **validating** Excel files, with built-in support for **Persian (Jalali) calendar**, **grouped headers**, **template binding**, and **in-memory metadata caching**.

If you're building a DDD/CQRS-based application and need to generate Excel reports or import data from user-uploaded Excel files, FastExcel is built for you.

---

## ✨ Features

| Feature | Description |
| :--- | :--- |
| 📤 **Export** | Generate Excel files from any list of DTOs/Models. |
| 📥 **Import** | Read Excel files with automatic header detection and type conversion. |
| 🏷️ **Attribute-based Configuration** | Use `[Display]`, `[ExcelColumn]`, `[HasExcelGroup]`, `[Hidden]` to control output. |
| 🎨 **Grouped Headers** | Multi-level (merged) headers with color palette. |
| 📅 **Persian Date Support** | Built-in conversion between Gregorian and Jalali calendars. |
| ⚡ **Metadata Cache** | In-memory cache makes repeated exports **5-10x faster**. |
| 🔄 **Async/Await** | Fully async API for high-performance scenarios. |
| 📋 **Template Binding** | Replace `{{PropertyName}}` placeholders in Excel templates. |
| ✅ **Validation Reports** | Import with row-by-row validation and detailed error reports. |
| 🎯 **DDD/CQRS Friendly** | Works seamlessly with DTOs, Commands, and Queries. |

---

## 📦 Packages

| Package | Description | Dependencies |
| :--- | :--- | :--- |
| **FastExcel.Abstractions** | Contracts, Attributes, Options. | None |
| **FastExcel.Core** | Core implementation (uses EPPlus). | EPPlus |
| **FastExcel.DependencyInjection** | DI extensions for `IServiceCollection`. | Microsoft.Extensions.DI |

---

## 🚀 Quick Start

### Installation

```bash
dotnet add package FastExcel.Core
dotnet add package FastExcel.DependencyInjection

Project Structure
FastExcel.sln
├── src/
│   ├── FastExcel.Abstractions/       (Contracts, Attributes, Options)
│   ├── FastExcel.Core/               (Implementation with EPPlus)
│   └── FastExcel.DependencyInjection/(DI extensions)
└── samples/
    └── FastExcel.SampleConsole/      (Runnable examples)

    
Requirements
.NET 10 (or later)

EPPlus 7.x (will be installed as a dependency)

License: MIT

 Contributing
Contributions are welcome! If you find a bug or have a feature request, please open an issue.

Fork the repository.

Create a feature branch (git checkout -b feature/amazing-feature).

Commit your changes (git commit -m 'Add amazing feature').

Push to the branch (git push origin feature/amazing-feature).

Open a Pull Request.

This project is licensed under the MIT License — see the LICENSE.txt file for details.

 Contact
Author: Mahdi Amini

Email: Mahdi.Amini.dev@gmail.com

GitHub: @MahdiAmini98
