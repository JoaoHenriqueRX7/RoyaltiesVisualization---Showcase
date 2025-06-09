<h1 align="center">📊 Celesta Royalties Visualization + AI Insights</h1>

<p align="center">
  <strong>Dashboard & AI-powered API for royalty tracking at Celesta Mining (Vila&nbsp;Velha, Brazil)</strong>
</p>

> ⚠️ **Quick heads-up:** this repo contains only the first phase of the project that is Royalties Visualizatio, the complete project will have also ore extracion visualization. Focus was on core functionality and AI integration.

---

🛑 **Important note:**  
This code was developed exclusively for Celesta. It is shared here as a showcase only (non-commercial). Source code and architecture are under NDA.  
Questions? → [joaohenrique@jhbdev.com.br](mailto:joaohenrique@jhbdev.com.br)

---
https://drive.google.com/file/d/1l1ixHr8fz6upJyyQZpHPrZffIbSHUBaY/view?usp=share_link
[![User - Chat Text](https://drive.google.com/uc?export=view&id=1YJV8ZBjNma1OAktYyjvI0qIjd8fGJDLB)](https://drive.google.com/uc?export=view&id=1YJV8ZBjNma1OAktYyjvI0qIjd8fGJDLB)
https://drive.google.com/file/d/1shvEAxX5Kun661_xIsmujEUOK-y0pIdV/view?usp=share_link

| page | Description |
|------------|-------------|
| [![User - Chat Text](https://drive.google.com/uc?export=view&id=1YJV8ZBjNma1OAktYyjvI0qIjd8fGJDLB)](https://drive.google.com/uc?export=view&id=1YJV8ZBjNma1OAktYyjvI0qIjd8fGJDLB) | User chat interface: conversation with agent (text) |
| [![User - Chat Voice](https://drive.google.com/uc?export=view&id=1EOjNcHOmwXiYjPz_gXJXcvZeN0OfSXBg)](https://drive.google.com/uc?export=view&id=1EOjNcHOmwXiYjPz_gXJXcvZeN0OfSXBg) | User chat interface: conversation with agent (voice enabled via ElevenLabs) |
| [![Admin - Edit Agent](https://drive.google.com/uc?export=view&id=1shvEAxX5Kun661_xIsmujEUOK-y0pIdV)](https://drive.google.com/uc?export=view&id=1shvEAxX5Kun661_xIsmujEUOK-y0pIdV) | Admin panel: editing an existing agent |
| [![Admin - Create Agent](https://drive.google.com/uc?export=view&id=1l1ixHr8fz6upJyyQZpHPrZffIbSHUBaY)](https://drive.google.com/uc?export=view&id=1l1ixHr8fz6upJyyQZpHPrZffIbSHUBaY) | Admin panel: creating a new agent for a tenant |

## Interface demonstration  
👉 **[Watch the demo](https://youtu.be/your-demo-link)**

---

## 📸 High-Level Architecture  

[![Architecture Diagram](https://drive.google.com/uc?export=view&id=1lpHn0sdCWlOImzG5AaS5rhWcuYaO84-M)](https://drive.google.com/uc?export=view&id=1lpHn0sdCWlOImzG5AaS5rhWcuYaO84-M)
---

## 🚀 Why?

Celesta Royalties Visualization + AI is an MVP built for Celesta Mining to provide a secure, flexible dashboard and an AI-powered assistant for real-time royalty oversight.
It turns complex data—like invoices, shareholder positions, and FX rates—into actionable insights, with natural-language Q&A and voice interaction.
The architecture is modular and future-proof, with FastAPI + RAG enabling chat, document parsing, and seamless scaling—finally moving the operation beyond spreadsheets.
Looking ahead, the same stack will power full ore-pipeline management and operational visualization, giving Celesta one clear view across the entire mining lifecycle.

### 💰 **Real-time financial governance**  
Executives can monitor royalties owed, paid, taxes, and FX rates in real time — no spreadsheets required.

### 🎛 **Interactive dashboards & advanced filters**  
Dynamic filtering by date, shareholder, currency, invoice — lightning fast.

### 🔐 **Enterprise-grade security**  
JWT-based authentication, RBAC, encrypted data at rest, and multi-tenant readiness.

### 🌍 **Automatic currency conversion**  
Up-to-date USD ↔ BRL exchange rates via external API — seamlessly integrated.

---

## 🛠️ How It’s Built (Tech Stack)

| Layer | Technology |
|-------|------------|
| Frontend | React • Vite • Tailwind • Framer Motion |
| Charts | @nivo/bar • @nivo/pie • Recharts |
| State/Data | @tanstack/react-query • Zod |
| Backend | FastAPI • SQLAlchemy • PostgreSQL • RAG pipeline for AI assistant |
| Auth | JWT (python-jose) |
| Currency | ExchangeRate.host API + Redis cache |
| Infra | Docker containers on AWS EC2 behind an ALB |

---

## 🔗 Core Modules

- **User Dashboard:** key metrics, charts, and AI chat  
- **Invoices:** full CRUD, multi-share support, PDF export  
- **Shareholders:** investor management and reporting  
- **REST API:** currency conversion, royalties aggregation, AI-powered endpoints

---

## 🗂️ Interaction Flow

1. **Login** → JWT issued from `/auth/token`  
2. **Dashboard** loads real-time metrics + exchange rates  
3. User filters data / edits invoices or shareholders  
4. Optional: AI Chat → voice or text interaction  
5. RAG-enhanced responses streamed live

---

## 🔑 Essential API Endpoints

| Endpoint | Purpose |
|----------|---------|
| `POST /auth/token` | issue JWT |
| `GET /dashboard/summary` | aggregated royalties |
| `GET /invoices` | list invoices |
| `POST /invoices` | create invoice |
| `GET /shareholders` | list shareholders |
| `POST /ai/query` | AI assistant query (voice or text) |

---

## 📌 Roadmap

- ore pipeline management and visualization 
- Bulk document uploads (CSV/PDF)  
- Usage-based billing & rate limiting  
- SAP integrations  
- White-label mobile app

---

## 🙌 Interested?

📧 [joaohenrique@jhbdev.com.br](mailto:joaohenrique@jhbdev.com.br)

---

## 📜 Licensing

All documentation and visuals here are under **CC-BY-NC-SA 4.0**.  
Source code is private and protected under NDA with Celesta.

---

Thanks for visiting!
