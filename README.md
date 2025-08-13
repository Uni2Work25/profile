# Harshit Aggarwal - AI Email Marketing Portfolio

A modern, responsive portfolio website showcasing AI-powered email marketing expertise with interactive features and comprehensive case studies.

## 🚀 Live Demo

Visit the live portfolio: [harshit-portfolio.netlify.app](https://harshit-portfolio.netlify.app)

## ✨ Features

- **Multi-page Portfolio**: 6 dedicated pages (Home, About, Services, Portfolio, Email Preview, Contact)
- **Creative Loading Screen**: Animated progress loader with email marketing theme
- **Live Email Preview**: Interactive email template showcase with category filtering
- **Animated Metrics**: Real-time counter animations and progress bars
- **Responsive Design**: Optimized for all devices with mobile-first approach
- **Dark Theme**: Professional dark navy design with blue/purple accents
- **Performance Optimized**: Fast loading with Vite build optimization

## 🛠 Tech Stack

### Frontend
- **React 18** with TypeScript
- **Vite** for lightning-fast development and builds
- **Tailwind CSS** for utility-first styling
- **Wouter** for lightweight routing
- **Radix UI + shadcn/ui** for accessible components
- **Framer Motion** for smooth animations
- **TanStack Query** for data management

### Backend (Development)
- **Express.js** with TypeScript
- **PostgreSQL** with Drizzle ORM
- **Zod** for runtime validation

### Deployment
- **Netlify** with global CDN
- **Continuous deployment** from Git
- **Environment variable** management
- **Custom domain** support

## 📁 Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Page components (Home, About, etc.)
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utilities and configurations
├── server/                # Backend Express.js application
├── shared/               # Shared types and schemas
├── netlify.toml         # Netlify deployment configuration
└── _redirects          # SPA routing for Netlify
```

## 🎨 Key Pages

### Home Page
- Hero section with AI-powered email marketing expertise
- Animated performance metrics
- Service overview cards
- Results showcase with proven statistics

### About Page
- Professional background and experience
- Interactive skill bars with animations
- Career timeline with achievements
- Educational background and certifications

### Services Page
- 6 comprehensive email marketing services
- Process workflow visualization
- Pricing and feature details
- Proven results metrics

### Portfolio Page
- 6 detailed case studies with real metrics
- Client testimonials with star ratings
- Technology stack for each project
- ROI and performance improvements

### Email Preview Page
- Live email template preview system
- Category-based template filtering (Welcome, Promotional, Newsletter)
- Interactive template selection
- Free template download functionality

### Contact Page
- Professional contact form with validation
- Multiple contact methods
- Social media integration
- Free consultation booking

## 🚀 Deployment on Netlify

### Automatic Deployment
1. Connect your repository to Netlify
2. Set build command: `npm run build`
3. Set publish directory: `dist/public`
4. Deploy automatically on git push

### Manual Deployment
```bash
# Build the project
npm run build

# Deploy to Netlify (using Netlify CLI)
netlify deploy --prod --dir=dist/public
```

### Environment Variables
Set these in Netlify dashboard for full functionality:
- `DATABASE_URL` - PostgreSQL connection string
- `NODE_ENV` - Set to "production"

## 🎯 Performance Features

- **Fast Loading**: Vite-optimized builds with code splitting
- **SEO Optimized**: Meta tags and structured data
- **Mobile First**: Responsive design with touch-friendly interactions
- **Accessibility**: WCAG compliant with screen reader support
- **Cache Optimization**: Strategic caching for static assets

## 📊 Analytics & Metrics

The portfolio showcases real performance metrics:
- 500+ Email campaigns completed
- 35% Average open rate improvement
- 12% Conversion rate optimization
- 50+ Satisfied clients served
- $2M+ Revenue generated through campaigns

## 🎨 Design System

- **Colors**: Dark navy base with blue (#4285F4) and purple (#8B5CF6) accents
- **Typography**: Inter font family for modern readability
- **Spacing**: Consistent 8px grid system
- **Components**: shadcn/ui component library
- **Animations**: Smooth transitions with Framer Motion

## 📱 Responsive Breakpoints

- **Mobile**: 320px - 767px
- **Tablet**: 768px - 1023px  
- **Desktop**: 1024px - 1439px
- **Large Desktop**: 1440px+

## 🔧 Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📈 Future Enhancements

- [ ] Contact form integration with Netlify Forms
- [ ] Blog section with CMS integration
- [ ] Advanced email template customization
- [ ] Client portal with project tracking
- [ ] A/B testing showcase tools
- [ ] Real-time analytics dashboard

## 📄 License

This project is built for Harshit Aggarwal's professional portfolio. All rights reserved.

## 🤝 Contact

For inquiries about email marketing services or portfolio development:

- **Email**: harshit@emailexpert.com
- **Phone**: +1 (555) 123-4567
- **Location**: New York, NY
- **Response Time**: Within 24 hours

---

*Built with ❤️ using modern web technologies and deployed on Netlify*