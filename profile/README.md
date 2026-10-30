<div align="center">

<img src="https://raw.githubusercontent.com/Trexoncorp/.github/main/profile/assets/banner.svg" alt="Trexon — practical infrastructure for modern applications" width="100%" />

**Focused .NET libraries. Clear APIs. Less setup.**

Use one package or bring the pieces together — from configuration and logs to a working HTTP service.

[Explore the libraries](#the-building-blocks) · [Run the demo](#see-it-working) · [Get started](#add-what-you-need)

![.NET 8+](https://img.shields.io/badge/.NET-8%2B-8B5CF6?style=flat-square&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square)
![Available on NuGet](https://img.shields.io/badge/Available_on-NuGet-004880?style=flat-square&logo=nuget&logoColor=white)

</div>

---

## The building blocks

Small, composable libraries for everyday application infrastructure. Each package
has its own documentation and can be installed directly from NuGet.

| Library | What it brings to your application | NuGet |
| --- | --- | --- |
| **[Trexon.Configuration](https://github.com/Trexoncorp/Trexon.Configuration)** | Typed settings, defaults, environment variables, `.env` files, and validation. | [![NuGet](https://img.shields.io/nuget/v/Trexon.Configuration?style=flat-square&color=8B5CF6)](https://www.nuget.org/packages/Trexon.Configuration) |
| **[Trexon.Logging](https://github.com/Trexoncorp/Trexon.Logging)** | Structured events, contextual properties, console and JSON output, and data redaction. | [![NuGet](https://img.shields.io/nuget/v/Trexon.Logging?style=flat-square&color=8B5CF6)](https://www.nuget.org/packages/Trexon.Logging) |
| **[Trexon.Data](https://github.com/Trexoncorp/Trexon.Data)** | Short-lived EF Core sessions and supported schema updates for SQLite, PostgreSQL, and MySQL. | [![NuGet](https://img.shields.io/nuget/v/Trexon.Data?style=flat-square&color=8B5CF6)](https://www.nuget.org/packages/Trexon.Data) |
| **[Trexon.Web](https://github.com/Trexoncorp/Trexon.Web)** | Attribute-based routes, validation, Swagger, authentication modules, and typed WebSockets. | [![NuGet](https://img.shields.io/nuget/v/Trexon.Web?style=flat-square&color=8B5CF6)](https://www.nuget.org/packages/Trexon.Web) |

## See it working

**[Trexon.Demo → A notes API with a complete walkthrough](https://github.com/Trexoncorp/Trexon.Demo)**

Create a note in Swagger, save it to SQLite, trace the request in structured logs,
and restart the application to check that the data is still there.
The demo consumes the published NuGet packages.

```sh
git clone https://github.com/Trexoncorp/Trexon.Demo.git
cd Trexon.Demo
dotnet run
```

Open **http://127.0.0.1:5090/docs** and try the API.
The demo builds with **.NET SDK 10** and runs on **ASP.NET Core Runtime 8**.

| Try this | What you will see |
| --- | --- |
| Create and edit notes | Attribute-based endpoints and validated request models |
| Restart the service | Persistent SQLite data and a schema check at startup |
| Inspect `logs/demo.jsonl` | Business events and HTTP logs connected by request ID |
| Change `.env` | Typed settings with environment overrides and startup validation |

## Add what you need

From your .NET project directory, install the packages you want to use:

```sh
dotnet add package Trexon.Configuration --version 1.0.0
dotnet add package Trexon.Logging --version 1.0.0
dotnet add package Trexon.Data --version 1.0.0
dotnet add package Trexon.Web --version 1.0.0
```

Each library README includes a quick start, examples, and detailed documentation.
The demo shows how to compose all four in an application.

## Documentation & feedback

- **Learn:** start with the README in the library you are using.
- **Explore:** follow the [demo walkthrough](https://github.com/Trexoncorp/Trexon.Demo#demo-walkthrough).
- **Report a bug or suggest a feature:** open an issue in the relevant repository with a small example and the package version.

---

<div align="center">

**Build something useful. Keep the infrastructure understandable.**

[Repositories](https://github.com/orgs/Trexoncorp/repositories) · [Demo](https://github.com/Trexoncorp/Trexon.Demo) · [NuGet](https://www.nuget.org/profiles/anton_aleynichenko)

</div>
