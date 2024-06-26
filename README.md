# About

A Wongnok web application designed to foster a vibrant community of food enthusiasts in Thailand and beyond.

# 🌏[Check out my production server](https://kirato.cloud)

## How to start dev

0. Config .env file !

.env for local

```.env
NEXTAUTH_URL=http://localhost:3000
GOOGLE_CLIENT_ID=${get from google oauth}
GOOGLE_CLIENT_SECRET=${get from google oauth}
NEXTAUTH_SECRET=kiratopat
```

Or otherwise please contact me via Line ID : `kiratopat`


1. install pnpm for faster package management

```bash
$ npm install -g pnpm
```

2. install node packages

```bash
$ pnpm install
```

3. run Postgresql using docker

```bash
$ docker-compose up -d
```

4. push the Prisma schema state to the database

```bash
$ pnpm prisma db push
```

5. run dev server

```bash
$ pnpm dev
```

# pnpm cli

```bash
Install package
$ pnpm install

Start dev
$ pnpm dev

Start dev useing turbo pack (optional)
$ pnpm dev --turbo

Build project
$ pnpm build

Start server from builded project
$ pnpm start
```

ps. I use pnpm as node package management, you can use what you prefer (such as yarn, npm, bun, etc...)

# Prisma cli

Examples

Set up a new Prisma project

```bash
$ prisma init
```

Generate artifacts (e.g. Prisma Client)

```bash
$ prisma generate
```

Browse your data

```bash
$ prisma studio
```

Create migrations from your Prisma schema, apply them to the database, generate artifacts (e.g. Prisma Client)

```bash
$ prisma migrate dev
```

Pull the schema from an existing database, updating the Prisma schema

```bash
$ prisma db pull
```

Push the Prisma schema state to the database

```bash
$ prisma db push
```

Validate your Prisma schema

```bash
$ prisma validate
```

Format your Prisma schema

```bash
$ prisma format
```

Display Prisma version info

```bash
$ prisma version
```

Display Prisma debug info

```bash
$ prisma debug
```

# How to run Docker

Normal run

```bash
$ docker-compose up
```

Detached run

```bash
$ docker-compose up -d
```

## Tech Stack

- NEXTJS version 14.0.4
- Tailwind CSS + Daisy UI
- NextAuth.js
- Docker
- PostgresDB
- Linux server
