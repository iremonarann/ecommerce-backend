# E-Commerce Web Application — Backend

Bu proje, e-ticaret uygulamasının **ASP.NET Core tabanlı REST API** katmanıdır. Ürün, kategori, kullanıcı ve sipariş yönetimini sağlayan servisleri içerir ve Angular frontend uygulamasına servis verir.

**Frontend Projesi:** `ecommerce-frontend` (Angular)

---

## Features


### API Katmanı
- RESTful servis mimarisi
- Controller tabanlı yapı
- Middleware tabanlı hata ve istek yönetimi
- JSON veri iletişimi

### İş Katmanı (Business Layer)
- Abstract / Concrete katman ayrımı
- DTO yapıları
- Validation işlemleri
- Exception yönetimi
- Profil eşlemeleri (AutoMapper)

### Veri Katmanı
- Entity tabanlı modelleme
- Repository pattern yaklaşımı
- Konfigüre edilebilir veri erişim katmanı

### Sistem Altyapısı
- Çok katmanlı mimari
- SOLID prensiplerine uygun yapı
- Docker desteği
- Ortam bazlı yapılandırma (Development / Staging)

---

## Tech Stack
- ASP.NET Core 8.0
- C#
- Entity Framework Core
- AutoMapper
- FluentValidation

---

## Project Structure

```text
ECommerceSiteApi
├── Northwind.Api
│   ├── Controllers
│   ├── Middlewares
│   ├── Models
│   ├── Properties
│   ├── Program.cs
│   ├── appsettings.json
│   ├── appsettings.Development.json
│   ├── appsettings.Staging.json
│   └── Dockerfile
├── Northwind.Business
│   ├── Abstract
│   ├── Concrete
│   ├── Data
│   ├── Dtos
│   ├── Exceptions
│   ├── Profiles
│   └── Validators
└── Northwind.sln
```

---

## Getting Started

### Prerequisites
- .NET 8 SDK
- Microsoft SQL Server (MSSQL)

### Run (Development)
```bash
dotnet restore
dotnet run --project Northwind.Api
```
Application runs at:
https://localhost:5001

