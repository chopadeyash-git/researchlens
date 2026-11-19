# ResearchLens 🔍

ResearchLens is a modern, unified academic research platform that simplifies discovering, filtering, and understanding academic literature across multiple open repositories and publishers.

---

## ✨ Features

- **Multi-Source Paper Discovery**: Queries across multiple scientific data sources (arXiv, CrossRef, PubMed, Semantic Scholar, and CORE) in real time.
- **Deduplication & Smart Ranking**: Merges duplicate records across sources and ranks results by citations, recency, and abstract quality.
- **AI-Powered Synthesis**: Generates structured summaries and key takeaways (problem statement, methodology, contributions, results, limitations) using LLMs with smart rule-based fallbacks.
- **Platform Deep Links**: Provides one-click access to full texts, open-access PDFs, and direct search links for publisher portals.
- **Personal Research Library**: Save and organize papers locally with offline persistence.
- **Search History & Caching**: Fast querying with an in-memory server cache and saved local history.
- **Clean Responsive UI**: Modern dark/light interface built for desktop and mobile workflows.

---

## 🛠️ Architecture & Tech Stack

### Frontend
- **Languages**: HTML5, CSS3, JavaScript (Vanilla ES6+)
- **Storage**: Browser LocalStorage for library and search history
- **Design**: Responsive layout with modern styling and theme switching

### Backend
- **Runtime**: Node.js & Express
- **HTTP Client**: Axios
- **Parser**: xml2js, pdf-parse
- **AI Integrations**: Groq Cloud API, Ollama (local fallback), and rule-based heuristic parser

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- npm

### 1. Clone the repository
```bash
git clone https://github.com/chopadeyash-git/researchlens.git
cd researchlens
```

### 2. Backend Setup
```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder:
```env
PORT=5000
FRONTEND_URL=http://127.0.0.1:5500
GROQ_API_KEY=your_groq_api_key
SEMANTIC_API_KEY=optional_key
CORE_API_KEY=optional_key
```

Start the backend server:
```bash
npm start
```

### 3. Frontend Setup
Open `frontend/index.html` in your web browser or serve it using any static server:
```bash
npx serve frontend
```

---

## 👤 Author

- **Developer**: Yash Chopade
- **GitHub**: [@chopadeyash-git](https://github.com/chopadeyash-git)
- **Contact**: chopadeyash07@gmail.com

---

## 📄 License

This project is licensed under the MIT License.
