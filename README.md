# hello-dotnet

[![.NET CI/CD](https://github.com/Evgeny65ok/hello-dotnet/actions/workflows/ci.yml/badge.svg)](https://github.com/Evgeny65ok/hello-dotnet/actions/workflows/ci.yml)
![.NET](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet&logoColor=white)
![Release](https://img.shields.io/github/v/release/Evgeny65ok/hello-dotnet?color=success)

Учебный проект: **CI/CD на C#/.NET** с автоматической сборкой и публикацией в **GitHub Releases**.

## Что делает пайплайн
- `dotnet restore`, `dotnet build`, `dotnet test` (xUnit) — CI-проверки
- `dotnet publish` — сборка в папку `publish/`
- Упаковка в `hello-dotnet.tar.gz`
- Публикация в Release при push тега `v*`

## Скриншоты
**Actions:**
<img width="1624" height="732" alt="Снимок экрана 2026-09-25 112441" src="https://github.com/user-attachments/assets/6ad5b4d4-8086-4f36-9563-54ee82d2dad6" />


**Release v1.0.0:**

<img width="1499" height="829" alt="Снимок экрана 2026-09-25 112505" src="https://github.com/user-attachments/assets/fc9e5f6a-56ad-4a35-bf41-ab94be2baab1" />

## Использование
Скачай `hello-dotnet.tar.gz` из [Releases](../../releases), распакуй и запусти:

```powershell
Invoke-WebRequest -Uri "https://github.com/Evgeny65ok/hello-dotnet/releases/download/v1.0.0/hello-dotnet.tar.gz" -OutFile "hello-dotnet.tar.gz"
tar -xzf hello-dotnet.tar.gz
.\hello-dotnet.exe
