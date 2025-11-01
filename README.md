# 🎯 ECF Dashboard

<div align="center">

**Real-time Cognitive Sovereignty Monitoring System**

![Status](https://img.shields.io/badge/status-in%20development-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript)

[العربية](#النسخة-العربية) • [English](#english-version)

</div>

---

## 📋 Overview

The **ECF Dashboard** is a real-time monitoring application that tracks and visualizes cognitive sovereignty metrics in human-AI interactions. It provides actionable insights into:

- 🧠 **Systems Tracking**: Monitor total active cognitive systems
- 📊 **Sovereignty Metrics**: Measure cognitive autonomy levels (0-100%)
- 📉 **Gap Analysis**: Identify knowledge gaps and improvement areas
- 🌍 **Bilingual Interface**: Full Arabic and English support

---

## 🏗️ Architecture

### Part of the Evolutionary Core Framework

```
ecf-theory (Theoretical Foundation)
    ↓
    ├─→ ecf-study-aperture (RCT Data)
    ├─→ ecf-study-interactions (Pattern Analysis)
    ↓
ecf-dashboard (Real-time Metrics) ← You are here
    ↓
Actionable Insights
```

### Related Projects
- **[ecf-theory](https://github.com/riteofrene/ecf-theory)** - Theoretical framework
- **[ecf-study-aperture](https://github.com/riteofrene/ecf-study-aperture)** - Safe Aperture RCT study
- **[ecf-study-interactions](https://github.com/riteofrene/ecf-study-interactions)** - Interaction patterns research

---

## ✨ Features

### Core Functionality
- ✅ **Real-time Dashboard**: Live metrics visualization
- ✅ **System Management**: Add, track, and monitor multiple systems
- ✅ **Sovereignty Scoring**: Automated calculation of cognitive sovereignty levels
- ✅ **Gap Detection**: Identify and quantify knowledge gaps
- ✅ **Progress Tracking**: Monitor improvements over time

### Technical Features
- ⚡ **Fast & Responsive**: Built with React 18
- 🎨 **Modern UI**: Tailwind CSS styling
- 📱 **Mobile-First**: Responsive design for all devices
- 🌐 **i18n Ready**: Arabic/English language switching
- 📊 **Data Visualization**: Interactive charts with Recharts

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/riteofrene/ecf-dashboard.git
cd ecf-dashboard

# Install dependencies
npm install

# Start development server
npm start
```

The dashboard will open at `http://localhost:3000`

---

## 📦 Tech Stack

### Core
- **React 18** - UI framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling

### Data & Visualization
- **Recharts** - Chart library
- **Lucide React** - Icon system

### State Management
- **React Hooks** - useState, useEffect, useReducer
- **Context API** - Global state (no localStorage/sessionStorage)

---

## 📊 Dashboard Components

### 1. Systems Panel (إجمالي الأنظمة)
```javascript
{
  totalSystems: number,
  activeSystems: number,
  activePercentage: number
}
```

### 2. Sovereignty Gauge (السيادة المعرفية)
```javascript
{
  sovereigntyScore: number (0-100),
  yearlyAverage: number,
  trend: 'up' | 'down' | 'stable'
}
```

### 3. Gaps Analyzer (متوسط الفجوات)
```javascript
{
  averageGaps: number (0-100),
  improvementNeeded: boolean,
  suggestions: string[]
}
```

---

## 🎨 UI Screenshots

### Arabic Interface
```
┌─────────────────────────────────────┐
│  لوحة التحكم الرئيسية               │
├─────────────────────────────────────┤
│  🧠 إجمالي الأنظمة: 0               │
│  📊 السيادة المعرفية: 0%            │
│  📉 متوسط الفجوات: 0%               │
│                                     │
│  [إضافة نظام جديد]                  │
└─────────────────────────────────────┘
```

---

## 🔌 API Integration

### Data Connectors
The dashboard can integrate with:

```javascript
// Example: Fetch data from research projects
const fetchSovereigntyData = async () => {
  const aperture = await fetch('/api/ecf-study-aperture/metrics');
  const interactions = await fetch('/api/ecf-study-interactions/patterns');
  
  return calculateSovereignty(aperture, interactions);
};
```

### Future Integrations
- [ ] Real-time data from Safe Aperture study
- [ ] Pattern analysis from Interaction study
- [ ] Export to Zenodo for archival
- [ ] PDF report generation

---

## 🛠️ Development

### Project Structure
```
ecf-dashboard/
├── src/
│   ├── components/
│   │   ├── SystemsPanel.tsx
│   │   ├── SovereigntyGauge.tsx
│   │   └── GapsAnalyzer.tsx
│   ├── hooks/
│   │   └── useSovereigntyMetrics.ts
│   ├── locales/
│   │   ├── ar.json
│   │   └── en.json
│   └── App.tsx
├── public/
├── package.json
└── README.md
```

### Available Scripts

```bash
# Development
npm start           # Start dev server
npm test            # Run tests
npm run build       # Production build

# Code Quality
npm run lint        # Run ESLint
npm run format      # Format with Prettier
```

---

## 📖 Usage Guide

### Adding a New System

1. Click **"إضافة نظام جديد"** (Add New System)
2. Enter system details
3. Monitor metrics in real-time

### Understanding Metrics

**Cognitive Sovereignty (0-100%)**
- 0-25%: Heavy AI dependence
- 26-50%: Moderate autonomy
- 51-75%: Good self-direction
- 76-100%: High cognitive sovereignty

**Knowledge Gaps (0-100%)**
- 0-25%: Minimal gaps
- 26-50%: Some improvement needed
- 51-75%: Significant gaps
- 76-100%: Critical attention required

---

## 🌍 Localization

### Supported Languages
- 🇸🇦 Arabic (العربية) - Primary
- 🇬🇧 English - Secondary

### Adding a New Language

```javascript
// src/locales/fr.json
{
  "dashboard.title": "Tableau de bord",
  "systems.total": "Systèmes totaux",
  ...
}
```

---

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md).

### Ways to Contribute
- 🐛 Report bugs
- 💡 Suggest features
- 📝 Improve documentation
- 🌍 Add translations
- 🎨 Enhance UI/UX

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

## 🔗 Links

- **Project Homepage**: [riteofrene.github.io/ecf-theory](https://riteofrene.github.io/ecf-theory)
- **Research Portfolio**: [github.com/riteofrene](https://github.com/riteofrene)
- **Issues**: [Report a bug](https://github.com/riteofrene/ecf-dashboard/issues)
- **Discussions**: [Join the conversation](https://github.com/riteofrene/ecf-dashboard/discussions)

---

## 📬 Contact

For questions about the dashboard or research collaboration:

- Open an issue in this repository
- Visit our [main profile](https://github.com/riteofrene)
- Check the [ECF Theory documentation](https://github.com/riteofrene/ecf-theory)

---

## 🎓 Citation

If you use this dashboard in your research:

```bibtex
@software{ecf_dashboard_2025,
  title = {ECF Dashboard: Cognitive Sovereignty Monitoring System},
  author = {Rite of Renaissance},
  year = {2025},
  url = {https://github.com/riteofrene/ecf-dashboard}
}
```

---

<div align="center">

**Built with 🧠 for cognitive sovereignty**

[⭐ Star this repo](https://github.com/riteofrene/ecf-dashboard) • 
[🐛 Report Bug](https://github.com/riteofrene/ecf-dashboard/issues) • 
[💡 Request Feature](https://github.com/riteofrene/ecf-dashboard/issues)

</div>

---

## النسخة العربية

<div dir="rtl">

# 🎯 لوحة التحكم ECF

**نظام مراقبة السيادة المعرفية في الوقت الفعلي**

---

## 📋 نظرة عامة

لوحة التحكم ECF هي تطبيق مراقبة فوري يتتبع ويصور مقاييس السيادة المعرفية في تفاعلات الإنسان مع الذكاء الاصطناعي.

### المزايا الرئيسية

- 🧠 **تتبع الأنظمة**: مراقبة إجمالي الأنظمة المعرفية النشطة
- 📊 **مقاييس السيادة**: قياس مستويات الاستقلالية المعرفية (0-100%)
- 📉 **تحليل الفجوات**: تحديد الفجوات المعرفية ومجالات التحسين
- 🌍 **واجهة ثنائية اللغة**: دعم كامل للعربية والإنجليزية

---

## 🚀 البدء السريع

### المتطلبات
- Node.js 18+
- npm أو yarn

### التثبيت

```bash
# استنساخ المشروع
git clone https://github.com/riteofrene/ecf-dashboard.git
cd ecf-dashboard

# تثبيت المكتبات
npm install

# تشغيل الخادم التطويري
npm start
```

ستفتح اللوحة على `http://localhost:3000`

---

## 📊 مكونات اللوحة

### 1. لوحة الأنظمة
عرض إجمالي الأنظمة المعرفية المفعّلة والنشطة

### 2. مقياس السيادة
قياس مستوى الاستقلالية المعرفية بنسبة مئوية

### 3. محلل الفجوات
تحديد الفجوات المعرفية ومستوى التحسين المطلوب

---

## 🔗 المشاريع المرتبطة

- **[ecf-theory](https://github.com/riteofrene/ecf-theory)** - الإطار النظري
- **[ecf-study-aperture](https://github.com/riteofrene/ecf-study-aperture)** - دراسة الفتحة الآمنة
- **[ecf-study-interactions](https://github.com/riteofrene/ecf-study-interactions)** - دراسة أنماط التفاعل

---

## 📄 الترخيص

MIT License - للتفاصيل راجع ملف [LICENSE](LICENSE)

---

## 📬 التواصل

للأسئلة حول اللوحة أو التعاون البحثي:
- افتح issue في هذا المشروع
- زر [صفحتنا الرئيسية](https://github.com/riteofrene)

</div>

---

<div align="center">

**صُنع بـ 🧠 من أجل السيادة المعرفية**

</div>
