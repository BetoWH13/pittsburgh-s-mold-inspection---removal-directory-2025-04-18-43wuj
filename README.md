# Pittsburgh's Mold Inspection & Removal Directory

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A comprehensive directory website showcasing mold inspection and removal services in Pittsburgh, featuring a responsive 3-column grid layout and easy-to-navigate categories.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources & Support](#resources--support)

## Overview

This directory website provides a user-friendly platform for finding mold inspection and removal services in Pittsburgh. The responsive design ensures optimal viewing across all devices, while the intuitive navigation system helps users quickly find the services they need.

## Features

- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Service provider details pages
- Contact forms
- Mobile-friendly design
- SEO optimization
- Fast loading times

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/pittsburgh-mold-directory.git

# Navigate to project directory
cd pittsburgh-mold-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
├── public/
│   ├── images/
│   └── assets/
├── src/
│   ├── components/
│   ├── data/
│   ├── styles/
│   └── pages/
├── config/
├── package.json
└── README.md
```

## Customization Guide

### Adding Directory Items

1. Navigate to `src/data/directory-items.js`
2. Add new items following this format:

```javascript
{
  id: "unique-id",
  name: "Business Name",
  category: "Inspection",
  address: "123 Main St, Pittsburgh, PA",
  phone: "(412) 555-0123",
  website: "https://example.com",
  description: "Business description here"
}
```

### Modifying Categories

Edit categories in `src/data/categories.js`:

```javascript
export const categories = [
  "Inspection",
  "Removal",
  "Testing",
  "Prevention"
];
```

### Updating Hero Section

1. Open `src/components/Hero.js`
2. Modify the content:

```javascript
<div className="hero">
  <h1>Your New Headline</h1>
  <p>Your new subheading</p>
</div>
```

### Customizing Colors

Edit `src/styles/variables.scss`:

```scss
$primary-color: #your-color;
$secondary-color: #your-color;
$accent-color: #your-color;
```

## Deployment

### Building for Production

```bash
# Create production build
npm run build

# Test production build locally
npm run serve
```

### Deployment Options

1. **Netlify**
   - Connect your GitHub repository
   - Set build command: `npm run build`
   - Set publish directory: `dist`

2. **Vercel**
   - Install Vercel CLI: `npm i -g vercel`
   - Deploy: `vercel`

## Custom Domain Setup

1. Purchase domain name
2. Add DNS records:
   ```
   Type  Name  Value
   A     @     76.76.21.21
   CNAME www   yourdomain.com
   ```
3. Configure in deployment platform
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Build Failures**
   - Check Node.js version
   - Clear npm cache: `npm cache clean --force`
   - Delete node_modules and reinstall

2. **Style Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify SCSS compilation

3. **Data Not Updating**
   - Clear localStorage
   - Check data file syntax
   - Verify import paths

## Resources & Support

- [Documentation Wiki](https://github.com/yourusername/pittsburgh-mold-directory/wiki)
- [Issue Tracker](https://github.com/yourusername/pittsburgh-mold-directory/issues)
- [Contributing Guidelines](CONTRIBUTING.md)

### Support Channels

- Email: support@example.com
- Discord: [Join Server](https://discord.gg/example)
- Twitter: [@DirectorySupport](https://twitter.com/DirectorySupport)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

© 2023 Pittsburgh's Mold Inspection & Removal Directory. All rights reserved.