# AI-Powered Hotel Booking Aggregator

## Tech Stack
- **Backend:** NestJS + TypeScript + Prisma + PostgreSQL
- **Frontend:** Next.js 15 + TypeScript + Tailwind CSS + shadcn/ui
- **Auth:** JWT (access + refresh tokens)
- **AI:** Anthropic Claude API
- **Hosting:** Railway (backend + DB), Vercel (frontend)
- **Storage:** Cloudflare R2
- **Email:** Resend

## Getting Started

### Prerequisites
- Node.js LTS (v20+)
- Docker Desktop
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/AshaEdwin003/AI-Powered-Hotel-Booking-Aggregator.git
cd AI-Powered-Hotel-Booking-Aggregator

# Backend setup
cd backend
npm install
cp .env.example .env
docker compose up -d    # Start PostgreSQL
npx prisma migrate dev  # Run database migrations
npm run start:dev       # Start development server

# Frontend setup
cd ../frontend
npm install
cp .env.example .env.local
npm run dev