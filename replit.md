# Overview

CLEANWISE is a mobile car detailing service application built with a modern full-stack architecture. The application provides a comprehensive platform for customers to book various car detailing services, view service packages, read reviews, and contact the business. It features a responsive React frontend with shadcn/ui components and an Express.js backend with PostgreSQL database integration.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety
- **Routing**: Wouter for client-side routing (lightweight alternative to React Router)
- **State Management**: TanStack Query (React Query) for server state management and caching
- **UI Framework**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with custom design tokens and CSS variables for theming
- **Form Handling**: React Hook Form with Zod validation for type-safe form validation
- **Build Tool**: Vite for fast development and optimized production builds

## Backend Architecture
- **Framework**: Express.js with TypeScript for API development
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Database**: PostgreSQL with Neon Database as the cloud provider
- **Schema Validation**: Zod schemas shared between frontend and backend
- **Development**: Hot reload with Vite middleware integration for seamless development experience

## Data Storage Solutions
- **Primary Database**: PostgreSQL hosted on Neon Database
- **ORM**: Drizzle ORM with schema-first approach
- **Migration Management**: Drizzle Kit for database schema migrations
- **Development Fallback**: In-memory storage implementation for development/testing

## API Design
- **Architecture**: RESTful API with Express.js
- **Endpoints**: 
  - `/api/bookings` - CRUD operations for service bookings
  - `/api/contact` - Contact inquiry management
- **Data Validation**: Zod schemas for request/response validation
- **Error Handling**: Centralized error handling middleware
- **Logging**: Custom request/response logging for API endpoints

## Key Features
- **Service Booking System**: Multi-step booking form with validation
- **Service Packages**: Express Detail, Deep Clean, and Luxury Detail packages
- **Customer Reviews**: Display and management of customer testimonials
- **Gallery**: Showcase of before/after photos and service imagery
- **Contact Management**: Contact form with inquiry tracking
- **Mobile-First Design**: Responsive design optimized for mobile devices

## Development Environment
- **Replit Integration**: Configured for Replit development environment
- **Hot Reload**: Vite-powered development server with HMR
- **TypeScript**: Full TypeScript support across frontend and backend
- **Path Aliases**: Configured import aliases for clean code organization

# External Dependencies

## Database Services
- **Neon Database**: PostgreSQL cloud database provider
- **Connection**: Uses `@neondatabase/serverless` for optimized serverless connections

## UI Component Libraries
- **Radix UI**: Headless UI primitives for accessibility and functionality
- **Lucide React**: Icon library for consistent iconography
- **shadcn/ui**: Pre-built component library combining Radix UI with Tailwind CSS

## Development Tools
- **Vite**: Build tool and development server
- **Replit Plugins**: Custom Replit integration for development environment
- **PostCSS**: CSS processing with Tailwind CSS and Autoprefixer

## Validation and Forms
- **Zod**: Runtime type validation and schema definition
- **React Hook Form**: Form state management and validation
- **@hookform/resolvers**: Integration between React Hook Form and Zod

## Styling and Design
- **Tailwind CSS**: Utility-first CSS framework
- **Class Variance Authority**: Utility for creating component variants
- **clsx**: Conditional className utility
- **tailwind-merge**: Utility for merging Tailwind classes

## State Management
- **TanStack Query**: Server state management, caching, and synchronization
- **React Context**: Local state management for UI components

## Date and Utility Libraries
- **date-fns**: Date manipulation and formatting
- **nanoid**: Unique ID generation