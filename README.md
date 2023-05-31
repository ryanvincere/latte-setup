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
