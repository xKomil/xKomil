<div align="center">

# Hi 👋, I'm Kamil

### Junior Gen AI Specialist @ Warta

Poland · I build things that put language models to work, and ship them to real users.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-kamil--plocki-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kamil-plocki/)
[![Email](https://img.shields.io/badge/Email-kamilplocki13@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:kamilplocki13@gmail.com)

</div>

---

## 🚀 What I'm building

### 🎵 [Niespodzianka Muzyczna](https://niespodziankamuzyczna.pl) &nbsp;<sub>· live · commercial</sub>

A personalised song as a gift. You answer a few questions about the person, pick a
style — ballad, pop, rap, disco polo — and the lyrics are written from your answers,
with one free revision. AI composes the music and the vocal, a human checks the result,
and about 24 hours later you get an MP3 plus a printable PDF gift card with a QR code
to the track. Singles from 39.99 zł, EP and full-album tiers on the way.

The genuinely hard part is the vocal: most engines read Polish lyrics with an American
accent and no emotion, so picking and driving the audio models is most of the work.

### 💪 [E.V.](https://hey-ev.vercel.app) &nbsp;<sub>· live · private repo</sub>

A health app for a two-person household, built around **EV**, an AI assistant you can
type or talk to. She plans training and food, logs what you tell her (weight, sleep,
meals) and judges the numbers against your actual goal. Workouts with progression and
deload, a meal calendar for two (shared dinners, separate breakfasts sized to each
person's calories), a pantry read off fridge photos and a shared shopping list.

Built with **Next.js** on Vercel, **Supabase** with row-level security throughout, and
**Google Gemini** including the Live API. A few pieces I like:

- **Voice mode runs browser → Google directly.** The server only mints a single-use
  ephemeral token with the model, system prompt and tool list locked in, so the browser
  never holds an API key and can't swap in its own prompt. Every tool call still
  round-trips to the server, so writes happen under the user's own RLS.
- **The smart scale feeds itself.** Xiaomi Home → Apple Health → an iOS Shortcut posts
  weight, body fat, lean mass and steps to a token-authenticated endpoint, written by
  one `security definer` Postgres function, so a public endpoint never holds credentials
  that bypass RLS.
- **Safe to talk to in a shared flat.** Before EV first changes a training plan on a
  given day it saves yesterday's version; deleting anything needs an explicit "yes", and
  a restore shows exactly what will change before it touches anything.

### 🛂 [GuessThePassport](https://guessthepassport.vercel.app) &nbsp;<sub>· live · [open source](https://github.com/xKomil/GuessThePassport)</sub>

A mobile web game: guess the country from its passport. The name is blurred, so all you
have is the coat of arms and the language. A first-try guess on the cover scores 100,
a second try with the data page as a hint scores 50, and a round of ten ends on a Top 10
leaderboard. Next.js 16, React 19, Tailwind 4, Framer Motion and Supabase, with RLS
that allows public reads and inserts into the leaderboard, and nothing else.

---

## 🧰 Tech I reach for

**Gen AI**

![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

**Web**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

**Data & analytics**

![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![SAP HANA](https://img.shields.io/badge/SAP_HANA-0FAAFF?style=flat-square&logo=sap&logoColor=white)

**Ways of working** — Agile (Scrum, Kanban) · Jira · application testing

---

## 📚 A few public repos

| | |
|---|---|
| [**brain-tumor-detector**](https://github.com/xKomil/brain-tumor-detector) | Tumour classification from MRI scans |
| [**Machine-Learning-Web-App**](https://github.com/xKomil/Machine-Learning-Web-App) | Streamlit app estimating income, trained on the 2023 Stack Overflow survey |
| [**Data-Science**](https://github.com/xKomil/Data-Science) | Notebooks, Power BI and VBA from my analytics work |
| [**KoktajLove**](https://github.com/xKomil/KoktajLove) | Cocktail app in TypeScript |
| [**Filmweb-webscrapper**](https://github.com/xKomil/Filmweb-webscrapper) | Scrapes film ratings and returns them as JSON |

---

<div align="center">

🎓 **MSc student in Data Analysis** · BSc in Economic Informatics — University of Łódź

<br />

<img src="https://streak-stats.demolab.com?user=xKomil&locale=en&mode=daily&theme=dracula&hide_border=false&border_radius=5" height="150" alt="streak graph" />

</div>
