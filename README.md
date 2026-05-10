# LeedsWeb3 - Enterprise Web3 Consultancy Landing Page

A production-ready landing page for LeedsWeb3, an enterprise Web3 consultancy, recruitment, and education firm based in Leeds. Built with Next.js 14, Tailwind CSS, and Supabase.

## Features

- **Ultra-modern Design**: Dark theme with slate-950 background, neon blue/indigo glowing borders, and subtle grid backgrounds
- **Responsive Layout**: Fully responsive design optimized for all devices
- **Interactive Components**: 
  - Sticky navigation with mobile menu
  - Hero section with animated text and stats
  - Three-pillar service showcase
  - Interactive Leeds Sandbox with project tabs
  - Lead generation form with validation
  - YouTube section placeholder for Leeds Web3 TV
- **Database Integration**: Full Supabase integration with 4 tables for lead management
- **Production Ready**: Optimized for Vercel deployment with proper environment configuration

## Tech Stack

- **Frontend**: Next.js 14 (App Router), TypeScript, Tailwind CSS
- **Icons**: Lucide React
- **Database**: Supabase (PostgreSQL)
- **Deployment**: Vercel-ready

## Database Schema

The application includes 4 main tables:

1. **consultancy_leads** - Business consultancy inquiries
2. **talent_pool_applications** - Developer job applications
3. **academy_enrolments** - Student education enrollments
4. **hackathon_registrants** - Event registrations

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- Supabase account (for database)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd leedsweb3
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.local.example .env.local
```

4. Configure your Supabase credentials in `.env.local`:
```env
NEXT_PUBLIC_SUPABASE_URL=https://your-project-id.supabase.co
SUPABASE_SERVICE_ROLE_KEY=your-service-role-key-here
```

5. Set up your Supabase database:
   - Run the SQL migration script: `supabase_schema.sql`
   - Enable Row Level Security (RLS) policies are included in the schema

### Running the Application

1. Start the development server:
```bash
npm run dev
```

2. Open [http://localhost:3000](http://localhost:3000) in your browser

### Building for Production

```bash
npm run build
npm start
```

## Deployment

### Vercel Deployment

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Configure environment variables in Vercel dashboard
4. Deploy!

### Environment Variables Required

- `NEXT_PUBLIC_SUPABASE_URL` - Your Supabase project URL
- `SUPABASE_SERVICE_ROLE_KEY` - Your Supabase service role key

## API Endpoints

- `POST /api/submit-lead` - Submit consultancy leads
- `POST /api/submit-talent` - Submit talent applications  
- `POST /api/submit-enrollment` - Submit academy enrollments
- `POST /api/submit-hackathon` - Submit hackathon registrations

## Project Structure

```
src/
├── app/
│   ├── api/                 # API routes
│   ├── globals.css          # Global styles
│   ├── layout.tsx          # Root layout
│   └── page.tsx            # Home page
├── components/
│   ├── Navigation.tsx      # Navigation component
│   ├── Hero.tsx            # Hero section
│   ├── ThreePillars.tsx    # Services showcase
│   ├── LeedsSandbox.tsx    # Project showcase
│   ├── LeadGenForm.tsx     # Contact form
│   ├── YouTubeSection.tsx  # YouTube placeholder
│   └── Footer.tsx          # Footer
└── lib/
    └── supabase.ts         # Supabase client & types
```

## Customization

### Colors & Theme

The theme uses custom Tailwind colors defined in `tailwind.config.js`:
- `neon-blue` - #00d4ff
- `neon-indigo` - #6366f1
- `dark-slate` - #0f172a

### Components

All components are modular and can be easily customized:
- Modify component props to change content
- Update Tailwind classes for styling changes
- Add new components following the existing pattern

## Security

- Row Level Security (RLS) enabled on all tables
- Service role key used for server-side operations
- Input validation on all API endpoints
- SQL injection protection through Supabase

## Performance

- Optimized images and assets
- Lazy loading components
- Efficient database queries
- Production-ready build configuration

## Support

For support and questions:
- Email: info@leedsweb3.com
- Phone: +44 (0) 113 123 4567

## License

© 2024 LeedsWeb3. All rights reserved.

---

**Built with ❤️ for the Leeds Web3 community**
# leedsweb3
# leedsweb3
