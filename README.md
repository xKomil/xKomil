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

### 💪 [E.V.](https://ev-e.netlify.app) &nbsp;<sub>· live · private repo</sub>

A health coach for a two-person household — workout plans and sessions, nutrition
logging with photo analysis, an AI coach you can actually talk to, and a gamification
layer that scores itself from data the app already has.

Built with **Next.js** on Netlify, **Supabase** with row-level security throughout, and
**Google Gemini** including the Live API. Two pieces I like:

- **Voice mode runs browser → Google directly**, because Netlify Functions can't hold a
  WebSocket. The server's only job is minting a single-use ephemeral token with the
  model, system prompt and tool list locked in — the browser never holds an API key and
  can't substitute its own prompt. Every tool call still round-trips to the server, so
  writes happen under the user's own RLS.
- **Steps sync from an iPhone with nothing to install.** An iOS Shortcut posts Apple
  Health step counts to a token-authenticated endpoint. The write goes through one
  `security definer` Postgres function, so an endpoint that is public by construction
  never holds credentials that bypass RLS.

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
