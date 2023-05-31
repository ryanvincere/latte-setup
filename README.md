# latte-setup

### Install dependencies
`pnpm i`

### Setup connection
Create database at https://planetscale.com/


### Configure environment variables.
There is an `.env.example` in the root directory you can use for reference
- `cp .env.example .env`
- Replace DATABASE_URL from planetscale

### Migrate database
- Change directory to packages/db
- `pnpm db:generate` -> Generate prisma client
- `pnpm db:push` -> Generate database/migrate
- `pnpm db:seed` -> Running seeder

### Running project

- `pnpm dev`
- http://localhost:5556 (Prisma Studio)
- http://localhost:3000/ (Next JS) (create .env file inside app/apps/nextjs folder, and define SENDGRID_API_KEY and which value from test.js)
- Mobile (If error when running pnpm dev, please run `npx expo start --ios` inside app/apps/expo folder, and run `pnpm dev` again)

