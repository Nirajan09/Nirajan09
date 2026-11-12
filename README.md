<div align="center">

# Nirajan Tiwari

**Full-Stack Developer** at Cherdung Info Tech · Kathmandu, Nepal  
`React · Next.js · TypeScript · Django / DRF`

<p align="center">
  <a href="https://nirajantiwari.com.np"><img src="https://img.shields.io/badge/Portfolio-nirajantiwari.com.np-00F2FE?style=for-the-badge&logo=googlechrome&logoColor=080C14" alt="Portfolio"></a>
  <a href="https://github.com/Nirajan09"><img src="https://img.shields.io/badge/GitHub-Nirajan09-8B5CF6?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="GitHub"></a>
  <a href="https://www.linkedin.com/in/nirajan-tiwari"><img src="https://img.shields.io/badge/LinkedIn-Nirajan_Tiwari-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:nirajantiwari09@gmail.com"><img src="https://img.shields.io/badge/Email-Contact_Me-F59E0B?style=for-the-badge&logo=gmail&logoColor=080C14" alt="Email"></a>
</p>

</div>

### About

<div align="center">
  <img src="assets/terminal.svg" alt="Nirajan Tiwari About Terminal" width="830">
</div>

<div align="center">
  <img src="assets/divider.svg" alt="Section Divider" width="830">
</div>

## Projects

<!-- BookRecommendationSystem -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/projects/book-recommendation-system-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/projects/book-recommendation-system-light.svg">
    <img src="assets/projects/book-recommendation-system-dark.svg" alt="BookRecommendationSystem" width="830">
  </picture>
</div>

<p align="center">
  <a href="https://book-recommendation-system-umber.vercel.app/"><img src="https://img.shields.io/badge/Live_Demo-Vercel-black?style=flat-square&logo=vercel" alt="Live Demo"></a>
  <a href="https://github.com/Nirajan09/BookRecommendationSystem"><img src="https://img.shields.io/badge/Source-GitHub-181717?style=flat-square&logo=github" alt="Source Code"></a>
  <img src="https://img.shields.io/github/last-commit/Nirajan09/BookRecommendationSystem?style=flat-square&color=00F2FE" alt="Last Commit">
  <img src="https://img.shields.io/github/languages/top/Nirajan09/BookRecommendationSystem?style=flat-square&color=8B5CF6" alt="Top Language">
  <img src="https://img.shields.io/github/stars/Nirajan09/BookRecommendationSystem?style=flat-square&color=F59E0B" alt="Stars">
</p>

<details>
<summary><b>Architecture &amp; Specs</b></summary>

```mermaid
flowchart TD
    Client["Client (React 19 + Vite + Tailwind)"]
    API["Backend (Django 5.2 + DRF)"]
    ML["Recommender (pandas, numpy, scipy, scikit-learn)"]
    DB[("Database (PostgreSQL / SQLite)")]
    Pay["Payment (Stripe / eSewa / Cash on Delivery)"]

    Client -->|"Token Auth, Cart, Wishlist, Reviews"| API
    Client -->|"Checkout"| Pay
    API -->|"Storefront & Admin Data"| DB
    API -->|"User Ratings"| ML
    ML -->|"Collaborative & Fallback Recs"| API
```

- **Hybrid Recommender**: User-based + item-based collaborative filtering with popular-books fallback (`pandas`, `numpy`, `scipy`, `scikit-learn`).
- **Storefront & Checkout**: Token auth, cart, wishlist, reviews, and Stripe / eSewa / cash-on-delivery payments.
- **Admin Dashboard**: Sales, revenue, best sellers, and low-stock alerts (SQLite in dev, PostgreSQL in prod).

</details>

<br>

<!-- JobVista -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/projects/job-vista-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/projects/job-vista-light.svg">
    <img src="assets/projects/job-vista-dark.svg" alt="JobVista" width="830">
  </picture>
</div>

<p align="center">
  <a href="https://job-portal-liard-one.vercel.app/"><img src="https://img.shields.io/badge/Live_Demo-Vercel-black?style=flat-square&logo=vercel" alt="Live Demo"></a>
  <a href="https://github.com/Nirajan09/job-portal"><img src="https://img.shields.io/badge/Source-GitHub-181717?style=flat-square&logo=github" alt="Source Code"></a>
  <img src="https://img.shields.io/github/last-commit/Nirajan09/job-portal?style=flat-square&color=00F2FE" alt="Last Commit">
  <img src="https://img.shields.io/github/languages/top/Nirajan09/job-portal?style=flat-square&color=8B5CF6" alt="Top Language">
  <img src="https://img.shields.io/github/stars/Nirajan09/job-portal?style=flat-square&color=F59E0B" alt="Stars">
</p>

<details>
<summary><b>Architecture &amp; Specs</b></summary>

```mermaid
flowchart TD
    Candidate["Candidate"]
    Recruiter["Recruiter"]
    Next["Next.js 16 / React 19 (Server Actions, Radix UI)"]
    Clerk["Clerk Auth"]
    DB[("MongoDB Atlas (Mongoose)")]
    Storage["Supabase Storage (Resumes)"]
    Stripe["Stripe Checkout (Premium Membership)"]

    Candidate & Recruiter -->|"Authentication"| Clerk
    Candidate -->|"Resume Upload"| Storage
    Candidate -->|"Applications & Status Tracking"| Next
    Recruiter -->|"Membership Checkout"| Stripe
    Recruiter -->|"Job Posts & Review Profiles/Resumes"| Next
    Next -->|"Data Persistence"| DB
```

- **Dual Roles**: Candidate & recruiter onboarding, job filters, applications, status tracking, and profile/resume review.
- **Monetization & Storage**: Posting limits tied to Stripe membership tiers and Supabase Storage for resumes.
- **Core Stack**: Next.js 16 / React 19 server actions, Radix UI, Clerk auth, and MongoDB Atlas via Mongoose.

</details>

<br>

<!-- Pixify -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/projects/pixify-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/projects/pixify-light.svg">
    <img src="assets/projects/pixify-dark.svg" alt="Pixify" width="830">
  </picture>
</div>

<p align="center">
  <a href="https://image-sharing-platform-two.vercel.app/"><img src="https://img.shields.io/badge/Live_Demo-Vercel-black?style=flat-square&logo=vercel" alt="Live Demo"></a>
  <a href="https://github.com/Nirajan09/image-sharing-platform"><img src="https://img.shields.io/badge/Source-GitHub-181717?style=flat-square&logo=github" alt="Source Code"></a>
  <img src="https://img.shields.io/github/last-commit/Nirajan09/image-sharing-platform?style=flat-square&color=00F2FE" alt="Last Commit">
  <img src="https://img.shields.io/github/languages/top/Nirajan09/image-sharing-platform?style=flat-square&color=8B5CF6" alt="Top Language">
  <img src="https://img.shields.io/github/stars/Nirajan09/image-sharing-platform?style=flat-square&color=F59E0B" alt="Stars">
</p>

<details>
<summary><b>Architecture &amp; Specs</b></summary>

```mermaid
flowchart TD
    Client["Client (Next.js 16 + React 19 + Radix UI)"]
    API["API (Express 5 + Mongoose, JWT + bcrypt)"]
    Multer["Multer Memory Buffer"]
    Cloudinary["Cloudinary"]
    DB[("MongoDB")]

    Client -->|"Upload File"| Multer
    Multer -->|"Stream"| Cloudinary
    Cloudinary -->|"Asset Data"| API
    API -->|"Persist Metadata"| DB
    Client -->|"Update / Delete (Ownership-Checked)"| API
    API -->|"Remove Asset"| Cloudinary
    API -->|"Remove Record"| DB
```

- **Decoupled Media Pipeline**: Next.js 16 / Tailwind v4 frontend paired with an Express 5 / Mongoose REST API.
- **Direct Streaming & Auth**: JWT + bcrypt auth, Multer memory-buffered uploads streamed to Cloudinary, and ownership-checked cascading asset deletion.
- **Galleries**: Paginated community and per-user galleries with Radix UI dialogs.

</details>

<div align="center">
  <img src="assets/divider.svg" alt="Section Divider" width="830">
</div>

### Stack

<div align="center">
  <img src="assets/tech-orbit.svg" alt="Core Tech Stack" width="830">
</div>

<div align="center">
  <img src="assets/divider.svg" alt="Section Divider" width="830">
</div>

### Activity

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/output/github-contribution-grid-snake.svg">
  <img src="https://raw.githubusercontent.com/Nirajan09/Nirajan09/output/github-contribution-grid-snake-dark.svg" alt="Contribution Snake" width="830">
</picture>

<br><br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/metrics/github-metrics-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/metrics/github-metrics-light.svg">
  <img src="https://raw.githubusercontent.com/Nirajan09/Nirajan09/metrics/github-metrics-dark.svg" alt="Nirajan's GitHub Metrics" width="830">
</picture>

<br><br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=Nirajan09&theme=tokyonight&hide_border=true&background=080C14&ring=00F2FE&fire=F59E0B&currStreakLabel=00F2FE&currStreakNum=F8FAFC">
  <source media="(prefers-color-scheme: light)" srcset="https://streak-stats.demolab.com/?user=Nirajan09&theme=default&hide_border=true&background=F8FAFC&ring=0284C7&fire=D97706&currStreakLabel=0284C7&currStreakNum=0F172A">
  <img src="https://streak-stats.demolab.com/?user=Nirajan09&theme=tokyonight&hide_border=true&background=080C14&ring=00F2FE&fire=F59E0B&currStreakLabel=00F2FE&currStreakNum=F8FAFC" alt="GitHub Streak">
</picture>

</div>

<details>
<summary><b>3D Contribution Skyline</b></summary>

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/profile-3d-contrib/profile-night-rainbow.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Nirajan09/Nirajan09/profile-3d-contrib/profile-gitblock.svg">
    <img src="https://raw.githubusercontent.com/Nirajan09/Nirajan09/profile-3d-contrib/profile-night-rainbow.svg" alt="3D Contribution Skyline" width="830">
  </picture>
</div>

</details>

<div align="center">
  <img src="assets/divider.svg" alt="Section Divider" width="830">
</div>

<div align="center">
  <sub>Nirajan Tiwari · Kathmandu, Nepal</sub>
</div>
