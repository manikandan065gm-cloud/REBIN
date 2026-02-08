# ReBin – Smart E-Waste Recycling Platform

ReBin is an intelligent e-waste recycling system that makes responsible disposal simple, rewarding, and accessible. Built with modern web technologies, it helps users find nearby recycling bins, identify recyclable items using AI, and track their environmental impact.

## 🌟 Features

- **Smart Bin Finder**: Locate the nearest e-waste recycling bin with an interactive map
- **Real-time Capacity Tracking**: See bin fill levels and plan your recycling trip
- **AI Waste Detection**: Identify electronic items and get instant recycling value estimates
- **Rewards System**: Earn eco-points for your recycling contributions
- **Predictive Analytics**: Smart algorithms predict bin fill times and optimize collection routes

## 🚀 Tech Stack

- **Frontend**: React 19, TypeScript, React Router
- **Styling**: Tailwind CSS, shadcn/ui components
- **Backend**: Hono (Cloudflare Workers)
- **Database**: Cloudflare D1 (SQLite)
- **Maps**: Leaflet, React-Leaflet
- **Deployment**: Cloudflare Workers & Pages

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/rebin.git
cd rebin
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment:
```bash
# Create wrangler.toml for local development
cp wrangler.example.toml wrangler.toml
```

4. Create D1 database:
```bash
npx wrangler d1 create rebin-db
```

5. Update `wrangler.toml` with your database ID

6. Create R2 bucket:
```bash
npx wrangler r2 bucket create rebin-bucket
```

## 🛠️ Development

Run the development server:

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

## 🏗️ Build

Build for production:

```bash
npm run build
```

## 🚢 Deployment

Deploy to Cloudflare:

```bash
npx wrangler deploy
```

## 📁 Project Structure

```
rebin/
├── src/
│   ├── react-app/          # Frontend React application
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Route page components
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utility functions
│   ├── worker/            # Cloudflare Worker backend
│   ├── shared/            # Shared types and utilities
│   └── data/              # Static data files
├── public/                # Static assets
└── migrations/            # Database migrations
```

## 🌍 Environmental Impact

Electronic waste is one of the fastest-growing waste streams globally. ReBin helps:
- Reduce toxic waste in landfills
- Recover valuable materials for reuse
- Make recycling accessible and convenient
- Track and reward environmental contributions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Mocha](https://getmocha.com)
- UI components from [shadcn/ui](https://ui.shadcn.com)
- Icons from [Lucide](https://lucide.dev)
- Maps powered by [Leaflet](https://leafletjs.com)

## 📧 Contact

For questions or feedback, please open an issue on GitHub.

---

Made with 💚 for a sustainable future
