# Bol Verkoper Suite

Een complete front-end applicatie voor Bol.com verkopers, gebouwd met Next.js 14, TypeScript en Tailwind CSS.

## 🚀 Features

- **Modern Tech Stack**: Next.js 14 met App Router, TypeScript, Tailwind CSS
- **Responsive Design**: Mobile-first ontwerp met dark mode ondersteuning
- **PWA Ready**: Progressive Web App functionaliteit
- **Authenticatie**: Complete login/register flow met validatie
- **Dashboard**: Uitgebreid overzicht met KPI's en grafieken
- **Bestellingenbeheer**: Volledige bestelling workflow
- **Productbeheer**: Inline editing en bulk operaties
- **Micro-animaties**: Framer Motion voor soepele gebruikerservaring

## 🎨 Design System

- **Primaire kleur**: Bol Blauw (#0050D8)
- **Accent kleur**: Bol Geel (#FFD200)
- **Typografie**: Inter font family
- **Componenten**: Herbruikbare UI componenten met variant support

## 📁 Project Structuur

\`\`\`
src/
├── app/
│   ├── (protected)/          # Beveiligde routes
│   │   ├── layout.tsx        # Layout met sidebar en topbar
│   │   ├── page.tsx          # Dashboard
│   │   ├── bestellingen/     # Bestellingen pagina
│   │   └── producten/        # Producten pagina
│   ├── auth/                 # Authenticatie routes
│   │   ├── login/
│   │   └── register/
│   ├── layout.tsx            # Root layout
│   └── globals.css           # Globale styles
├── components/
│   ├── auth/                 # Authenticatie componenten
│   ├── layout/               # Layout componenten
│   └── ui/                   # Herbruikbare UI componenten
└── lib/
    └── utils.ts              # Utility functies
\`\`\`

## 🛠 Installatie

1. **Clone de repository**
   \`\`\`bash
   git clone <repository-url>
   cd bol-verkoper-suite
   \`\`\`

2. **Installeer dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Start development server**
   \`\`\`bash
   npm run dev
   \`\`\`

4. **Open in browser**
   \`\`\`
   http://localhost:3000
   \`\`\`

## 📦 Build voor Productie

\`\`\`bash
# Build de applicatie
npm run build

# Start productie server
npm start
\`\`\`

## 🔧 Configuratie

### Environment Variables

Maak een `.env.local` bestand aan in de root directory:

\`\`\`env
NEXT_PUBLIC_APP_URL=http://localhost:3000
\`\`\`

### PWA Configuratie

De applicatie is PWA-ready met een `manifest.json` bestand. Voor productie:

1. Voeg echte iconen toe aan `/public/`
2. Update de manifest.json met juiste URLs
3. Configureer service worker indien gewenst

## 🎯 Belangrijke Features

### Authenticatie
- **Login Form**: E-mail/wachtwoord met "onthouden" optie
- **Register Form**: Uitgebreide registratie met wachtwoord sterkte meter
- **Validatie**: Zod schema validatie met React Hook Form
- **Google OAuth**: Placeholder implementatie

### Dashboard
- **KPI Cards**: Animerende statistiek kaarten
- **Grafieken**: Recharts voor omzet en status visualisatie
- **Real-time Data**: Mock data met realistische updates

### Bestellingen
- **Tabbed Interface**: Filter op status (Open, Verzonden, etc.)
- **Bulk Acties**: Selecteer meerdere bestellingen
- **Pakketlabels**: PDF generatie simulatie
- **Zoekfunctie**: Real-time zoeken in bestellingen

### Producten
- **Inline Editing**: Direct bewerken van prijs en voorraad
- **Status Badges**: Visuele status indicatoren
- **Voorraad Alerts**: Automatische waarschuwingen
- **Bulk Upload**: Placeholder voor Excel import

## 🎨 Styling Guidelines

### Kleuren
\`\`\`css
/* Primaire kleuren */
--bol-blue: #0050D8;
--bol-yellow: #FFD200;

/* Gebruik in Tailwind */
bg-[#0050D8]    /* Bol blauw */
bg-[#FFD200]    /* Bol geel */
text-bol-blue   /* Custom utility class */
\`\`\`

### Componenten
- Gebruik `variant` props voor verschillende stijlen
- Hover effecten met `hover:scale-105` voor micro-animaties
- Consistent gebruik van `rounded-xl` voor cards
- Shadow system: `shadow-lg` voor cards, `shadow-xl` voor hover

### Responsive Design
- Mobile-first approach
- Sidebar collapseert naar overlay op mobile
- Grid layouts passen aan per breakpoint
- Touch-friendly button sizes

## 🔍 Testing

\`\`\`bash
# Run linting
npm run lint

# Type checking
npm run type-check
\`\`\`

## 📱 PWA Features

- **Offline Support**: Service worker voor caching
- **Install Prompt**: Native app-like installatie
- **Responsive**: Werkt op alle apparaten
- **Fast Loading**: Optimized assets en code splitting

## 🚀 Deployment

### Vercel (Aanbevolen)
\`\`\`bash
npm install -g vercel
vercel
\`\`\`

### Andere Platforms
De applicatie is compatible met alle Next.js hosting providers:
- Netlify
- AWS Amplify
- Railway
- DigitalOcean App Platform

## 🤝 Contributing

1. Fork het project
2. Maak een feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit je changes (`git commit -m 'Add some AmazingFeature'`)
4. Push naar de branch (`git push origin feature/AmazingFeature`)
5. Open een Pull Request

## 📄 License

Dit project is gelicenseerd onder de MIT License - zie het [LICENSE](LICENSE) bestand voor details.

## 🙏 Acknowledgments

- **Bol.com** voor de design inspiratie
- **Vercel** voor het Next.js framework
- **Tailwind CSS** voor het utility-first CSS framework
- **Framer Motion** voor de animaties
- **Recharts** voor de data visualisatie

---

**Gemaakt met ❤️ voor Bol.com verkopers**
