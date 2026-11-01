# 🏢 RealEstatePortfolio
 
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Rider](https://img.shields.io/badge/Rider-000000?style=for-the-badge&logo=jetbrains&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

**RealEstatePortfolio** je konzolna aplikacija razvijena u **C#** programskom jeziku na **.NET** platformi, namijenjena upravljanju portfeljem nekretnina. Projekt je nastao kao praktična nadogradnja na savladane osnove jezika, s ciljem primjene objektno orijentiranog programiranja (OOP), rada s kolekcijama, trajnog spremanja podataka u datoteke i obrade iznimki u stvarnom scenariju.

---

## ✨ Ključne funkcionalnosti

- **🔐 Korisnička autentifikacija:** Sustav prijave i registracije korisnika prije pristupa glavnom izborniku.
- **📋 CRUD operacije nad nekretninama:**
  - **Create:** Dodavanje novih nekretnina u portfelj (stanovi, kuće, poslovni prostori, zemljišta) s pripadajućim atributima (lokacija, kvadratura, cijena, status).
  - **Read:** Pregled svih nekretnina uz mogućnost filtriranja i pretraživanja po kriterijima.
  - **Update:** Ažuriranje cijene, dostupnosti ili opisa postojećih nekretnina.
  - **Delete:** Brisanje nekretnina iz aktivnog portfelja.
- **💾 Perzistencija podataka (File I/O):** Automatsko učitavanje i spremanje promjena u lokalne datoteke (`System.IO`) kako podaci ne bi bili izgubljeni nakon gašenja aplikacije.
- **🛡️ Sigurno izvođenje:** Validacija korisničkog unosa i upravljanje neočekivanim greškama pomoću `try-catch` blokova.

---

## 🧠 Primijenjeni koncepti i arhitektura

Projekt je strukturiran kroz principe čiste objektno orijentirane arhitekture:

| Koncept | Primjena u projektu |
| :--- | :--- |
| **Enkapsulacija i Properties** | Zaštita polja unutar modela (`Property`, `User`) i kontrola pristupa putem `get` / `set` akcesora |
| **Nasljeđivanje i Polimorfizam** | Bazna klasa za nekretnine i izvedene klase za specifične tipove objekata uz `virtual` i `override` metode |
| **Sučelja (Interfaces)** | Definiranje ugovora za servisne klase i upravljanje podacima (npr. `IPropertyService`) |
| **Enumi (Enumerations)** | Standardizacija tipova nekretnina (`PropertyType`) i statusa oglasa (`ListingStatus`) |
| **Kolekcije i LINQ** | Dinamičko upravljanje podacima u memoriji pomoću generičkih lista (`List<T>`) i brzo pretraživanje |
| **Rad s datotekama i Iznimke** | Trajna pohrana putem `System.IO` klasa uz robusnu obradu grešaka (`try-catch-finally`) |

---

## 🛠️ Korištene tehnologije i alati

- **Jezik:** C#
- **Framework:** .NET SDK
- **Razvojno okruženje (IDE):** JetBrains Rider
- **Verzioniranje:** Git & GitHub

---

## ⚙️ Kako pokrenuti kod lokalno?

1. **Kloniraj repozitorij:**
   ```bash
   git clone https://github.com/Carldev04/RealEstatePortfolio.git
   ```

   
