# 🌍 Geo.Location.Activities

**Geo.Location.Activities** is a custom UiPath activity that retrieves **geolocation data** (Country, City, TimeZone) based on an IP address using public APIs.

## 📦 Overview

This activity allows UiPath developers to:
- Detect the user's public IP automatically if not provided.
- Fetch accurate geolocation details (Country, City, and TimeZone).
- Return the result as a **dictionary** for easy consumption in workflows.

## ✅ Features

- 🧠 Auto-detect IP address (uses `https://api.ipify.org`)
- 🌍 Query IP geolocation from `http://ip-api.com/json/{ip}`
- 🔄 Return result as `Dictionary<string, string>`
- 🚀 Built for UiPath using .NET 6 and packaged via Visual Studio

## 🧾 Inputs

| Name      | Type   | Description                             |
|-----------|--------|-----------------------------------------|
| IPAddress | String | *(Optional)* IP address to query. If not set, it uses the current public IP. |

## 📤 Outputs

| Name     | Type    | Description                 |
|----------|---------|-----------------------------|
| Country  | String  | Country name of the IP      |
| City     | String  | City of the IP              |
| TimeZone | String  | Time zone of the IP         |
| Result   | Dictionary<string, string> | Contains keys: `Country`, `City`, `TimeZone` |

## ⚙️ Dependencies

- `Newtonsoft.Json`
- `System.Net.Http`
- Compatible with **UiPath Studio v2022.10+**
- .NET 6 runtime

## 💡 Use Cases

- Log user location in automation logs  
- Customize workflows based on user region  
- Filter data or UI elements depending on country

## 🔧 How to Install

1. Download the `.nupkg` file from the [Releases](https://github.com/AmrEzzatAbdo/Geo-Location-Lookup/releases).
2. Add the local path to UiPath Studio under **Manage Packages > Settings > User-defined package sources**.
3. Install it via **Manage Packages > Available > Your Custom Feed**.

## 📜 License

This project is licensed under the [MIT License].

## 👨‍💻 Author

Developed by **Amr Ezzat**

- LinkedIn: [linkedin.com/in/amr-ezzat](https://www.linkedin.com/in/amrezzatabdal-al/)
- Email: `amrezzat289@gmail.com`

---

> Feel free to contribute or open issues for improvements!
