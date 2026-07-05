# ⚖️ AlqistAss Assurance AI

**Plateforme rapide de traitement des sinistres & audit forensic**  
*Challenge d'Innovation & Assurances — CASH Assurances 2026*

[![Deploy](https://img.shields.io/badge/Deploy-Live-success?style=flat-square&color=00BFA5)](https://w4qhofgioe6qq.kimi.page)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-blue?style=flat-square&color=1565C0)](https://github.com/skacimo1985-star/alqistass-ai)
[![Supabase](https://img.shields.io/badge/Backend-Supabase-green?style=flat-square&color=3ECF8E)](https://qsjklqxdrrstethnqwsd.supabase.co)

---

## 🎯 Mission

AlqistAss (القسطاس) — *la balance IA des sinistres* — automatise la chaîne complète des sinistres pour **CASH Assurances (Algérie)** :

> **Déclaration → Analyse Forensique → Scoring Fraude → Décision d'Indemnisation → Archivage Blockchain**

---

## ✨ Fonctionnalités

| Module | Description |
|--------|-------------|
| 📊 **Dashboard** | Vue d'ensemble en temps réel des sinistres, KPIs et conformité |
| 🧠 **Prompt AI System** | 6 prompts spécialisés (Système, Fraude, Sinistres, Actuariat, Blockchain, Conformité) avec simulateur intégré |
| 📋 **Gestion Sinistres** | CRUD complet — déclaration, suivi, décision, archivage |
| 🚨 **Détection Fraude** | Scoring ISF (Indice de Suspicion de Fraude) 0-100% avec analyse ELA |
| 📈 **Actuariat IFRS 17** | Bilan actuariel, ratio combiné, solvabilité, rating |
| ⛓️ **Blockchain Audit** | Registre immuable SHA-256, consensus 2/3, traçabilité complète |
| ⚖️ **Conformité** | Cadre légal : Ord. 95-07, CIMA, IFRS 17, Loi 18-07 DZ, UAR |
| 👥 **Utilisateurs** | Gestion des rôles (Admin, Expert, Manager, Actuaire) |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                     FRONTEND                                │
│  React 19 + TypeScript + Vite + Tailwind CSS + shadcn/ui   │
│  Routing: react-router  |  State: React Hooks              │
│  Icons: lucide-react  |  Charts: recharts                   │
└────────────────────────┬────────────────────────────────────┘
                         │ HTTP / WebSocket
┌────────────────────────┴────────────────────────────────────┐
│                     BACKEND SUPABASE                        │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────┐  │
│  │   Auth JWT   │  │  PostgreSQL  │  │ Storage (docs)   │  │
│  │   OAuth 2.0  │  │    RLS       │  │   claim-docs     │  │
│  └──────────────┘  └──────────────┘  └──────────────────┘  │
│                                                             │
│  Tables: claims, fraud_scores, blockchain_blocks,          │
│          actuarial_reports, prompt_templates                 │
└─────────────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Couche | Technologie |
|--------|-------------|
| **Frontend** | React 19, TypeScript, Vite, Tailwind CSS 3.4, shadcn/ui |
| **Backend** | Supabase (PostgreSQL, Auth, Storage) |
| **Database** | PostgreSQL avec Row Level Security |
| **Auth** | Supabase Auth (JWT, OAuth 2.0) |
| **Storage** | Supabase Storage (documents sinistres) |
| **Hébergement** | Static Deploy (CDN global) |

---

## 🚀 Déploiement

### Variables d'environnement

```env
VITE_SUPABASE_URL=https://qsjklqxdrrstethnqwsd.supabase.co
VITE_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
```

### Installation locale

```bash
git clone https://github.com/skacimo1985-star/alqistass-ai.git
cd alqistass-ai
npm install
npm run dev
```

### Build production

```bash
npm run build
```

---

## 📁 Structure du projet

```
src/
├── App.tsx                 # Router principal
├── main.tsx                # Point d'entrée
├── index.css               # Styles globaux (thème dark AlqistAss)
├── lib/
│   ├── supabase.ts         # Client Supabase
│   └── utils.ts            # Utilitaires (cn, etc.)
├── hooks/
│   ├── useAuth.ts          # Auth state & operations
│   └── useClaims.ts        # CRUD sinistres Supabase
├── types/
│   ├── index.ts            # Types TypeScript métier
│   └── database.ts         # Types Supabase DB
├── components/
│   ├── Layout.tsx          # Layout avec sidebar
│   ├── StatCard.tsx        # Carte statistique
│   └── StatusBadge.tsx     # Badge de statut sinistre
└── pages/
    ├── Dashboard.tsx       # Tableau de bord
    ├── PromptAI.tsx        # Prompt AI System (cœur)
    ├── Claims.tsx          # Gestion des sinistres
    ├── FraudDetection.tsx  # Détection de fraude ISF
    ├── Actuarial.tsx       # Actuariat IFRS 17
    ├── Blockchain.tsx      # Blockchain audit trail
    ├── Compliance.tsx      # Conformité réglementaire
    ├── Login.tsx           # Page de connexion
    ├── Users.tsx           # Gestion utilisateurs
    └── SettingsPage.tsx    # Paramètres
```

---

## ⚖️ Conformité Réglementaire

| Réglementation | Statut |
|----------------|--------|
| Ordonnance 95-07 (Assurance DZ) | ✅ Conforme |
| Code CIMA | ✅ Conforme |
| UAR | ✅ Conforme |
| IFRS 17 | ✅ Conforme |
| Loi 18-07 DZ (Données) | ✅ Conforme |
| ISO 27001 / IEC 62443 | ✅ Conforme |

---

## 👤 Auteur

**MAHROUG ERRAS BELKACEM** — SIREP OASIS NEXUS WEFEH TECH DZ  
🏜️ Laghouat, Algérie | Brevet INAPI N° 5893/2025

---

<p align="center">
  <b>⚖️ AlqistAss Assurance AI — Challenge Innovation CASH Assurances × Innov & Insure 2026 — Soolvit</b>
</p>
