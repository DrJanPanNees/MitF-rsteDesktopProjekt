# Øvelse: GitHub Workflow & Domain Centric Mini-projekt (Maleren A/S)

## Metadata
- **Fag:** Systemudvikling (2. semester, Datamatiker)  
- **Varighed:** 2–3 timer (gruppearbejde)  
- **Hvorfor relevant?**  
  - GitHub er standardværktøjet i moderne softwareudvikling.  
  - Ved at forbinde **user stories → branches → kode → pull requests → review** oplever I et workflow tæt på det, professionelle teams bruger.  
  - Øvelsen kobler **Maleren A/S semesterprojektet** til hands-on praksis, så I både lærer om *Domain Centric design*, samarbejde og versionsstyring.  
- **Læringsmål:**  
  - Viden: Forstå sammenhængen mellem krav (user stories) og software-artefakter.  
  - Færdighed: Oprette, fordele og implementere user stories i GitHub Projects med branches og PRs.  
  - Kompetence: Reflektere over MVP, teamwork og review-processer, samt relatere det til semesterprojektet.  

---

## Opgave – Trin for trin

### 1. Find jeres MVP (30 min)
- Læs casen **Maleren A/S** igennem.  
- Diskutér i gruppen: *Hvad er det mindst mulige produkt (MVP), der giver værdi for en kunde?*  
- Skriv 3–5 **user stories** i GitHub Project Board, fx:  
  - "Som kunde vil jeg kunne oprette en konto, så jeg kan handle online."  
  - "Som kunde vil jeg kunne lægge en vare i kurven."  
  - "Som kunde vil jeg kunne se den samlede pris i kurven."  
- Tilføj dem til jeres **Project Board** under kolonnen *To Do*.  

---

### 2. Fordel ansvar og opret branches (20 min)
- Fordel user stories mellem jer.  
- Opret en branch for hver user story, fx:  
  - `feature/register-user`  
  - `feature/add-to-cart`  
  - `feature/checkout-price`  
- Commit en README.md, hvor I kort beskriver jeres MVP.  

---

### 3. Implementer funktionerne i en Console App (60 min)
Lav en simpel **C# console app**. Hvert teammedlem arbejder på sin feature.  

Eksempler (kan udbygges med egne ideer):  

```csharp
// feature/register-user
Console.WriteLine("Indtast brugernavn:");
string username = Console.ReadLine();
Console.WriteLine($"Velkommen, {username}! Du er nu registreret.");
```

```csharp
// feature/add-to-cart
List<string> cart = new List<string>();
cart.Add("Maling 10L – Hvid");
Console.WriteLine("Vare tilføjet til kurv!");
```

```csharp
// feature/checkout-price
decimal total = 299.95m;
Console.WriteLine($"Din kurv koster i alt: {total} DKK");
```

💡 Husk at gemme funktionaliteten i klasser/metoder – så koden minder om det I senere skal bygge i semesterprojektet.  

---

### 4. Pull Request & Review (30 min)
- Når en feature er færdig, lav en **pull request** til main.  
- En anden i gruppen skal være **reviewer**.  
- Revieweren må gerne foreslå forbedringer (fx bedre navngivning eller flere tests).  
- Først når review er godkendt, merges branchen.  

---

### 5. Test og integrér jeres MVP (20 min)
- Når alle branches er mergede, kør hele programmet fra **main**.  
- Tjek at jeres MVP virker (kontooprettelse, kurv, pris osv.).  
- Opdater jeres Project Board: flyt user stories til *Done*.  

---

### 6. Refleksion (20 min)
Lav en kort refleksion (README.md eller separat fil):  
- Hvordan fungerede processen med user stories → kode → PR → review?  
- Hvad gik godt?  
- Hvad gik mindre godt?  
- Hvad frustrerede jer?  
- Hvad gjorde jer glade?  
- Hvordan kan workflowet forbedres i jeres semesterprojekt?  

---

## Succeskriterier
- 3–5 user stories skrevet i GitHub Projects.  
- Branches oprettet og koblet til user stories.  
- Console app implementeret som MVP.  
- Pull requests reviewed og mergede til main.  
- Refleksion afleveret i repoet.  

---

👉 Øvelsen tager **2–3 timer** og giver jer en smagsprøve på, hvordan et *Domain Centric* team kan arbejde i praksis – i miniatureformat.  
