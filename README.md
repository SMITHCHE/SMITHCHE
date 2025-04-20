// src/App.jsx
import React from "react";
import "./index.css";

export default function App() {
  return (
    <main className="min-h-screen bg-gradient-to-br from-white to-blue-50 text-gray-800 p-6">
      <div className="max-w-4xl mx-auto space-y-10">
        <header className="text-center">
          <h1 className="text-4xl font-bold mb-2">🌐 Tour Guide Exchange</h1>
          <p className="text-lg">Démonstration / Demo</p>
        </header>

        <section className="grid md:grid-cols-2 gap-8">
          <div>
            <h2 className="text-2xl font-semibold mb-2">🇫🇷 Échangez vos cryptos facilement avec Tour Guide Token (TGT)</h2>
            <p>
              Tour Guide Exchange est une plateforme innovante qui vous permet d’acheter,
              vendre et échanger des cryptomonnaies en toute sécurité, avec un focus
              particulier sur notre jeton utilitaire : <strong>TGT (Tour Guide Token)</strong>.
            </p>
          </div>
          <div>
            <h2 className="text-2xl font-semibold mb-2">🇺🇸 Easily trade your crypto with Tour Guide Token (TGT)</h2>
            <p>
              Tour Guide Exchange is an innovative platform that lets you buy, sell, and
              swap cryptocurrencies securely, with a special focus on our utility token:
              <strong> TGT (Tour Guide Token)</strong>.
            </p>
          </div>
        </section>

        <section className="bg-white rounded-2xl shadow p-6">
          <h3 className="text-xl font-bold mb-4">🚀 Fonctionnalités / Features</h3>
          <ul className="list-disc list-inside space-y-2">
            <li>💱 Échange rapide entre BTC, ETH, SOL, et TGT / Fast swap between BTC, ETH, SOL, and TGT</li>
            <li>🛡️ Sécurité renforcée / Reinforced security</li>
            <li>📲 Interface simple et intuitive / Simple and intuitive interface</li>
            <li>🗺️ Connecté à Haiticherie.net pour les services touristiques / Connected to Haiticherie.net for tourism services</li>
          </ul>
        </section>

        <section className="bg-white rounded-2xl shadow p-6">
          <h3 className="text-xl font-bold mb-4">🔁 Comment ça marche ? / How does it work?</h3>
          <ol className="list-decimal list-inside space-y-1">
            <li>Créez un compte / Create an account</li>
            <li>Déposez vos cryptos / Deposit your crypto</li>
            <li>Échangez contre TGT ou d'autres actifs / Swap with TGT or other assets</li>
            <li>Utilisez vos TGT pour réserver des tours ou des expériences locales / Use TGT to book tours or local experiences</li>
          </ol>
        </section>

        <section className="bg-white rounded-2xl shadow p-6">
          <h3 className="text-xl font-bold mb-4">🪙 À propos du TGT / About TGT</h3>
          <ul className="list-disc list-inside space-y-2">
            <li>Blockchain : <strong>Solana</strong></li>
            <li>Utilité : Paiement de services touristiques, jeu Tap-to-Earn, avantages spéciaux sur Haiticherie.net</li>
            <li>Bientôt listé publiquement / Soon to be listed publicly</li>
          </ul>
        </section>
      </div>
    </main>
  );
}

// src/main.jsx
import React from "react";
import ReactDOM from "react-dom/client";
import App from "./App.jsx";
import "./index.css";

ReactDOM.createRoot(document.getElementById("root")).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);

// index.html
<!doctype html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tour Guide Exchange</title>
  </head>
  <body>
    <div id="root"></div>
    <script type="module" src="/src/main.jsx"></script>
  </body>
</html>

// tailwind.config.js
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

// postcss.config.js
export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};

// index.css
@tailwind base;
@tailwind components;
@tailwind utilities;

