# 🧪 QA Automation – NUnit & Playwright (TuristickiHub mini)

## 📌 Opis
Ovaj repozitorijum sadrži automatizovane testove (backend + UI) za **TuristickiHub (manja verzija aplikacije)**, razvijene u okviru predmeta *Testiranje i kvalitet softvera*.

Fokus je na:
- testiranju REST API logike kroz NUnit
- testiranju ključnih korisničkih tokova kroz Playwright (E2E)

---

## 🧰 Tehnologije
- C# / ASP.NET Web API
- SQL Server LocalDB
- React (JS)
- **NUnit** (unit/integration tests)
- **Playwright** (E2E UI tests)

---

## ✅ NUnit (backend testovi)
Testovi pokrivaju tipične scenarije:
- uspešno dodavanje / izmena / brisanje entiteta (Ok)
- validacija obaveznih polja (BadRequest)
- rad sa nepostojećim ID-jem (NotFound)
- provera da su promene perzistirane (npr. brisanje iz baze)

Primeri testiranih modula:
- Agencije
- Putovanja
- Aktivnosti
- Recenzije
- Rezervacije

---

## 🌐 Playwright (E2E testovi)
E2E testovi simuliraju ponašanje korisnika kroz browser:
- navigacija kroz stranice
- unos u forme
- CRUD operacije (dodaj / izmeni / obriši)
- verifikacija da se UI ažurirao nakon akcije

---

## ⚙️ Pokretanje aplikacije (lokalno)

### 1️⃣ SQL Server LocalDB
```bash
sqllocaldb create Putovanje
sqllocaldb start Putovanje
```
### 2️⃣ Backend
```bash
cd Projekat/BackEnd/WebTemplate
dotnet run
```

### 3️⃣ Frontend
```bash
npm install
npm start
```

### ▶️ Pokretanje testova
### NUnit
```bash
dotnet test
```

### Playwright
```bash
npx playwright test
```
Napomena: Tokom razvoja testova Playwright može da se pokreće i u režimu Headless = false radi lakšeg debugovanja.

---

## 👩‍💻 Autori
- Anđela Stojanović
- Anastasija Trajković
