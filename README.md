## Next.js App Router Course - Starter

Final result of following the [nextJS introductin course](https://nextjs.org/learn)

Didn't actually do the SEO part (chapter 16). 

# How to run locally
You will need an .env file in the root of the project containing the following values : 
```
POSTGRES_URL="postgres://default:eEHTPlV1X4ur@ep-round-darkness-a4h7103t-pooler.us-east-1.aws.neon.tech:5432/verceldb?sslmode=require"

POSTGRES_PRISMA_URL="postgres://default:eEHTPlV1X4ur@ep-round-darkness-a4h7103t-pooler.us-east-1.aws.neon.tech:5432/verceldb?sslmode=require&pgbouncer=true&connect_timeout=15"

POSTGRES_URL_NO_SSL="postgres://default:eEHTPlV1X4ur@ep-round-darkness-a4h7103t-pooler.us-east-1.aws.neon.tech:5432/verceldb"

POSTGRES_URL_NON_POOLING="postgres://default:eEHTPlV1X4ur@ep-round-darkness-a4h7103t.us-east-1.aws.neon.tech:5432/verceldb?sslmode=require"

POSTGRES_USER="default"

POSTGRES_HOST="ep-round-darkness-a4h7103t-pooler.us-east-1.aws.neon.tech"

POSTGRES_PASSWORD="eEHTPlV1X4ur"

POSTGRES_DATABASE="verceldb"

AUTH_SECRET=UKRPttXNWIkvOJ+H0Rum7LjSMoZqtkL8JCiLg2zivNc=
```

The POSTGRES related varables are directly linked to my personal Vercel account, with some 
limits on the amount of storage & compute time. It is recommended to change these values to
your own database, but for example purposes, I don't mind sharing mine. It will probalbly 
expire one day, and I will not follow up on that issue. 

AUTH_SECRET is required for password hash. 

Once the .env file is done, make sure [NodeJS](https://nodejs.org/en/download/) is installed

Finally, run the following commands : 
``` 
npm install -g pnpm
pnpm install
pnpm dev
```
On your favourite browser, visit http://localhost:3000/
You can login using the following credentials : 
- Email : `user@nextmail.com`
- Password : `123456` 

# Deployed version 
Alternatively, I have deployed a version once again on my personnal Vercel account. Therefore 
subject to running out of free ressources. But it should be accessible at : https://next-js-dashboard-one-flame-72.vercel.app/
