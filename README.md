# HomePlus - Property Enhancement Platform

A comprehensive web application designed to help Indian middle-class homeowners discover personalized property enhancement solutions. The platform connects homeowners with expert-curated improvement ideas to make homes more attractive, valuable, and comfortable.

## 🌐 Live Demo

**Frontend**: deploy to Render or your preferred static host.

**Backend**: deploy the Spring Boot API to Render and connect it to Aiven MySQL.

## 📋 Project Overview

HomePlus is a property improvement recommendation platform that offers:

- **Personalized Solutions**: Customized recommendations based on property type, budget, and preferences
- **Expert Curation**: Best property improvement ideas curated for middle-class budgets
- **Value Enhancement**: Strategic improvements to increase property market value
- **Design Inspiration**: Beautiful design ideas tailored for Indian homes

## 🎯 Features

### For Homeowners
- Submit property details and requirements
- Get personalized improvement recommendations
- Access curated design inspiration
- Track improvement progress
- Connect with verified contractors
- Calculate project costs

### For Administrators
- Review homeowner submissions
- Curate recommendations
- Manage user accounts
- Analytics and reporting
- Content management
- Quality control

## 🛠️ Tech Stack

- **Frontend**: React 19.2.0
- **Routing**: React Router DOM 7.13.0
- **Build Tool**: Vite 8.0.0
- **Styling**: CSS3 with custom styling
- **Deployment**: Render

## 📁 Project Structure

```
homeplus-react/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Button.jsx
│   │   ├── Card.jsx
│   │   └── Footer.jsx
│   ├── pages/
│   │   ├── PropertyPlatform.jsx    # Landing page
│   │   ├── Welcome.jsx             # Welcome screen
│   │   ├── Login.jsx               # Authentication
│   │   ├── HomeownerForm.jsx       # Property submission
│   │   ├── HomeownerDashboard.jsx  # User dashboard
│   │   └── AdminDashboard.jsx      # Admin panel
│   ├── styles/
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/rakesh32026/HomePlus.git
cd homeplus-react
```

2. Install dependencies
```bash
npm install
```

3. Start the development server
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:5173`

### Frontend Environment Variables

For local development, the app uses the Vite proxy and talks to `http://localhost:8080` automatically.

For production on Render, set the frontend environment variable below so requests go to the deployed backend:

```bash
VITE_API_BASE_URL=https://<your-render-backend-service>/api
```

Also set this on the backend Render service so CORS allows the deployed frontend origin:

```bash
APP_CORS_ALLOWED_ORIGIN=https://<your-render-frontend-service>
```

If you deploy both frontend and backend on Render, the frontend should call the backend service URL directly through `VITE_API_BASE_URL`.

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## 📱 Application Routes

| Route | Description |
|-------|-------------|
| `/` | Landing page with platform overview |
| `/welcome` | Welcome screen with animations |
| `/login` | User authentication (Login/Signup) |
| `/homeowner-form` | Property details submission form |
| `/homeowner-dashboard` | Homeowner's personal dashboard |
| `/admin-dashboard` | Administrator control panel |

## 🎨 Key Improvement Categories

- Kitchen Renovation
- Bathroom Upgrade
- Living Room Makeover
- Bedroom Enhancement
- Flooring Replacement
- Wall Painting
- Electrical Upgrades
- Plumbing Improvements
- Home Automation
- Security Systems

## 👥 Team Members

- Rakesh - Full Stack Development
- Team Member 2 - UI/UX Design
- Team Member 3 - Frontend Development

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- React Team for the amazing framework
- Vite for the blazing fast build tool
- Vercel for seamless deployment

---

**Made with ❤️ for Indian Middle-Class Homes**
