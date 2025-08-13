# Overview

This is a personal portfolio website for Harshit Aggarwal, an AI-powered email marketing expert and PGDM student. The application showcases Harshit's expertise in creating AI-driven email campaigns, featuring live email preview functionality, performance analytics, and comprehensive service offerings. The portfolio demonstrates advanced email marketing capabilities with a focus on data-driven results and automation. The application is optimized for deployment on Netlify with modern static site hosting capabilities.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
The application uses a modern React-based single-page application (SPA) architecture built with TypeScript and Vite for fast development and optimal performance.

**UI Framework**: React 18 with TypeScript provides type safety and modern development patterns. The application uses Wouter for lightweight client-side routing instead of heavier alternatives like React Router.

**Styling System**: Tailwind CSS with a custom design system using CSS variables for consistent theming. The design follows a dark theme with blue and purple accent colors, implemented through the shadcn/ui component library built on Radix UI primitives.

**Component Library**: Radix UI primitives provide accessible, unstyled components that are then styled with Tailwind CSS through the shadcn/ui system. This ensures accessibility compliance while maintaining design consistency.

**State Management**: TanStack Query (React Query) handles server state management and data fetching, providing caching, background updates, and optimistic updates out of the box.

**Custom Components**: Specialized components include AnimatedCounter for performance metrics, SkillBar for animated skill demonstrations, and LoadingScreen for initial app loading with progress indication.

## Backend Architecture
The backend uses Express.js with TypeScript in a lightweight REST API structure, designed for development flexibility and production scalability.

**Server Framework**: Express.js provides the HTTP server foundation with TypeScript for type safety across the entire stack.

**Development Integration**: Vite middleware integration enables hot module replacement during development, allowing for seamless full-stack development experience.

**Storage Abstraction**: The application implements an abstracted storage interface (IStorage) with an in-memory implementation (MemStorage) for development. This pattern allows easy swapping to database implementations in production.

**Middleware Stack**: Custom logging middleware tracks API performance and responses, while error handling middleware provides structured error responses.

## Data Storage Solutions
The application is configured for PostgreSQL with Drizzle ORM, providing type-safe database operations and schema management.

**Database**: PostgreSQL configured for use with Neon serverless integration, allowing for scalable cloud database deployment.

**ORM**: Drizzle ORM provides type-safe database queries with schema introspection and migration management. The schema is defined in TypeScript and automatically generates types.

**Schema Design**: Currently includes a basic users table with authentication fields, designed to be extended with email marketing specific tables for campaigns, templates, subscribers, and analytics.

**Migration System**: Drizzle Kit manages database migrations with PostgreSQL dialect, ensuring database schema version control and deployment consistency.

## Authentication and Authorization
The application has a foundational authentication system built into the storage interface, designed for future expansion.

**User Management**: Basic user creation and retrieval functionality through the storage interface, with username-based lookup capabilities.

**Session Management**: Configuration includes connect-pg-simple for PostgreSQL-based session storage, though current implementation uses in-memory storage for development.

**Security Foundation**: Password handling and user identification structures are in place for implementing full authentication flows.

# External Dependencies

## UI and Component Libraries
- **Radix UI**: Complete suite of accessible, unstyled UI primitives including dialogs, dropdowns, tooltips, and form components
- **shadcn/ui**: Pre-styled component library built on Radix UI with Tailwind CSS integration
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens and responsive design capabilities
- **Lucide React**: Icon library providing consistent, customizable SVG icons throughout the application

## Development and Build Tools
- **Vite**: Modern build tool and development server with hot module replacement and optimized production builds
- **TypeScript**: Static type checking across frontend, backend, and shared code
- **ESBuild**: Fast JavaScript bundler used by Vite for rapid development and production builds

## Data Management
- **TanStack Query**: Server state management with caching, background updates, and data synchronization
- **Drizzle ORM**: Type-safe database ORM with PostgreSQL support and schema management
- **Drizzle Kit**: Database migration and schema management tools
- **Neon Database**: Serverless PostgreSQL database platform for cloud deployment

## Form and Validation
- **React Hook Form**: Performant form library with minimal re-renders and easy validation integration
- **Hookform Resolvers**: Integration layer between React Hook Form and validation libraries
- **Zod**: TypeScript-first schema validation with runtime type checking (via drizzle-zod integration)

## Development Environment
- **Modern Build Tools**: Vite with React plugins for fast development and optimized production builds
- **PostCSS**: CSS processing with Tailwind CSS and Autoprefixer plugins for browser compatibility

## Email and Communication (Configured)
- **SendGrid**: Email delivery service integration for contact forms and email notifications (included in dependencies for future implementation)

## Utility Libraries
- **Class Variance Authority**: Utility for creating component variants with conditional class names
- **clsx**: Conditional className utility for dynamic styling
- **date-fns**: Date manipulation and formatting library
- **Nanoid**: URL-safe unique string ID generator for various application needs