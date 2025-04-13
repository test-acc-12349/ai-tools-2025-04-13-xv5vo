# AI Tools Directory 🤖

> The ultimate directory of AI tools and resources for enhancing productivity and creativity.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization](#customization)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [Support](#support)

## Overview

AI Tools Directory is a curated collection of artificial intelligence tools and resources. The directory features a responsive 3-column grid layout, categorization system, and search functionality to help users discover the perfect AI tools for their needs.

## Features

- 📱 Responsive 3-column grid layout
- 🏷️ Category filtering (AI, New, Sale)
- 🔍 Search functionality
- 💨 Fast loading performance
- 🎨 Customizable styling
- 📊 SEO optimized
- 📱 Mobile-friendly design

## Demo

View the live demo: [https://ai-tools-directory.netlify.app](https://ai-tools-directory.netlify.app)

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   │   ├── Card.js
│   │   ├── Grid.js
│   │   ├── Hero.js
│   │   └── Search.js
│   ├── data/
│   │   └── tools.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization

### Adding Directory Items

Edit the `src/data/tools.json` file:

```json
{
  "tools": [
    {
      "id": "1",
      "name": "AI Writer Pro",
      "description": "Advanced AI writing assistant",
      "category": ["ai", "new"],
      "url": "https://example.com",
      "image": "/images/ai-writer.png"
    }
  ]
}
```

### Modifying Categories

Update the category array in `src/config/categories.js`:

```javascript
export const categories = [
  { id: 'ai', label: 'AI' },
  { id: 'new', label: 'New' },
  { id: 'sale', label: 'Sale' }
];
```

### Customizing Colors

Edit the CSS variables in `src/styles/main.css`:

```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --background-color: #f5f6fa;
  --text-color: #2c3e50;
}
```

### Updating Hero Section

Modify the Hero component in `src/components/Hero.js`:

```javascript
const Hero = () => {
  return (
    <div className="hero">
      <h1>AI Tools Directory</h1>
      <p>Discover the best AI tools for your needs</p>
    </div>
  );
};
```

## Deployment

### Netlify Deployment

1. Create a Netlify account
2. Connect your GitHub repository
3. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
4. Click "Deploy"

### Vercel Deployment

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel
```

## Custom Domain Setup

1. Purchase a domain from your preferred registrar
2. Add domain in your deployment platform (Netlify/Vercel)
3. Update DNS records:
   ```
   A Record: @ -> [deployment-platform-ip]
   CNAME: www -> [your-site-name].netlify.app
   ```
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Build Failures**
   - Check Node.js version compatibility
   - Verify all dependencies are installed
   - Review build logs for specific errors

2. **Styling Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify media queries

3. **Image Loading**
   - Confirm image paths are correct
   - Check image formats are supported
   - Verify image sizes are optimized

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Support

- 📧 Email: support@aitools.com
- 💬 Discord: [Join our community](https://discord.gg/aitools)
- 📚 Documentation: [docs.aitools.com](https://docs.aitools.com)
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/ai-tools-directory/issues)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)