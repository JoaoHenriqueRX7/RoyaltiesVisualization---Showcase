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

| Page | Description |
|------|-------------|
| ![Dashboard](https://via.placeholder.com/150) | Real-time overview of royalties owed/paid |
| ![Invoice CRUD](https://via.placeholder.com/150) | Full invoice management + PDF export |
| ![Shareholder Detail](https://via.placeholder.com/150) | Shareholder details & participation shares |
| ![AI Chat](https://via.placeholder.com/150) | AI-powered assistant for natural language queries |

## Interface demonstration  
👉 **[Watch the demo](https://youtu.be/your-demo-link)**

---

## 📸 High-Level Architecture  

[![Architecture Diagram]([https://via.placeholder.com/600x300)](https://via.placeholder.com/1200x600](https://drive.google.com/uc?export=view&id=1pPPMhQAQMNNI_a55dDZvKNXDd89C5q83)](https://drive.google.com/uc?export=view&id=1pPPMhQAQMNNI_a55dDZvKNXDd89C5q83))
---

## 🚀 Why Celesta Royalties Visualization?

### 🤖 **AI-Powered Business Insights**  
A built-in AI assistant (RAG-powered) enables natural language questions about royalties, invoices, shareholder balances, and financial trends. The assistant is available both within the dashboard and via the API — giving decision-makers fast, intuitive access to key data.

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

- Final UI/UX redesign (dark mode + responsive)  
- Bulk document uploads (CSV/PDF)  
- Usage-based billing & rate limiting  
- SAP & Power BI integrations  
- White-label mobile app (with AI voice assistant)

---

## 🙌 Interested?

📧 [joaohenrique@jhbdev.com.br](mailto:joaohenrique@jhbdev.com.br)

---

## 📜 Licensing

All documentation and visuals here are under **CC-BY-NC-SA 4.0**.  
Source code is private and protected under NDA with Celesta.

---

Thanks for visiting!
