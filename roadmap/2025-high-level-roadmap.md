\# 2025 – High-Level Roadmap



This roadmap describes \*\*phases\*\* and \*\*milestones\*\* for the Wine Marketplace project.  

Dates are approximate – focus is on sequence and learning, not strict deadlines.



---



\## Phase 1 – Foundation \& Environment



\*\*Goal:\*\* Clean separation of work vs personal, stable tooling, and basic structure.



\- ✅ Set up:

&nbsp; - Separate local folders for work \& personal (`D:\\Dev\\Personal`, `D:\\Dev\\Public`)

&nbsp; - Private code repo: `wine-marketplace`

&nbsp; - Public roadmap repo: `wine-marketplace-roadmap`

\- ✅ Configure:

&nbsp; - SSH keys (personal)

&nbsp; - Git remotes and profiles (personal vs work separation)

&nbsp; - GitHub Actions for weekly devlog

\- 🔜 Create solution skeleton:

&nbsp; - `WineMarketplace.sln` in the private repo root

&nbsp; - `src/`, `tests/`, `docs/` structure



---



\## Phase 2 – Backend Architecture (MVP)



\*\*Goal:\*\* Minimal but clean backend for managing wineries and wines.



\- Design core domain model:

&nbsp; - Winery, Wine, Region, Grape variety, Price, Stock

\- Implement basic services:

&nbsp; - CRUD for wineries and wines

&nbsp; - Simple filtering (by region, grape, style)

\- Technical tasks:

&nbsp; - ASP.NET Core Web API project

&nbsp; - EF Core setup (DbContext, migrations)

&nbsp; - Connection strings via User Secrets

&nbsp; - Basic logging \& error handling



---



\## Phase 3 – Admin Panel (Internal UI)



\*\*Goal:\*\* An internal admin UI for managing data.



\- Technology:

&nbsp; - React (likely Vite + TypeScript)

\- Features:

&nbsp; - Secure login (even if simple at first)

&nbsp; - List \& edit wineries and wines

&nbsp; - Basic filters and search

\- Integrations:

&nbsp; - Connect to backend API

&nbsp; - Handle loading, errors, and validation feedback



---



\## Phase 4 – Extended Features



\*\*Goal:\*\* Move closer to a usable marketplace MVP.



\- Add entities:

&nbsp; - Orders, Export requests, Customers, Shipments

\- Features:

&nbsp; - Basic order lifecycle

&nbsp; - Export status tracking

&nbsp; - Simple reporting (e.g. total bottles, revenue per region)

\- Technical:

&nbsp; - Pagination, sorting, filtering

&nbsp; - Possibly background jobs for longer operations



---



\## Phase 5 – Pre-production Hardening



\*\*Goal:\*\* Make the system stable enough for real test users.



\- Security review (auth, roles, input validation)

\- More detailed logging \& audit trails

\- Performance checks on main queries

\- Better error messages \& UX polishing in admin panel



---



\## How I Use This Roadmap



\- Large items live here (phases, milestones)

\- Weekly concrete progress goes into:

&nbsp; - `changelog/YYYY-MM-week-NN.md` (auto-created by GitHub Actions)

\- When priorities change, this file is updated – it’s a living document, not a fixed contract.



