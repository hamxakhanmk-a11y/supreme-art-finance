# Supreme Art Finance

Finance app for Supreme Art Private Limited.

Started as an exact copy of the Supreme Art Tracker app (full history included); the
tracker-specific features are being removed and finance features added in their place.

## Stack
- **Frontend**: Plain HTML/JS (`public/index.html`)
- **Backend**: Node.js + Express (`server.js`)
- **Database**: Neon Postgres (via `@neondatabase/serverless`)
- **Auth**: Google Sign-In + JWT session cookie
- **Hosting**: Vercel

## Local Development

1. Clone the repo
2. Install dependencies:
   ```
   npm install
   ```
3. Create a `.env` file in the root (see `.env.example` for every variable):
   ```
   DATABASE_URL=your_neon_connection_string
   GOOGLE_CLIENT_ID=your_google_oauth_client_id
   JWT_SECRET=a_long_random_string
   ```
4. Run locally:
   ```
   npm run dev
   ```
5. Open `http://localhost:3000`

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to vercel.com → New Project → Import your GitHub repo
3. Add the environment variables from `.env.example` in the Vercel dashboard
4. Deploy — Vercel auto-deploys on every push to main

## Making Changes

- Edit the code
- Push to GitHub (`git push`)
- Vercel auto-deploys within ~30 seconds
- No manual steps needed
