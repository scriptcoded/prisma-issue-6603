# Reproduction for Prisma issue 6603

https://github.com/prisma/prisma/issues/6603

## Bug description

When installing within a PNPM monorepo the generator isn't being run.

## How to reproduce

Reproduction coming in a few minutes (want the issue number)

1. Make sure PNPM is installed. (https://pnpm.io/installation)
2. Clone the reproduction repo
3. Enter the `app` directory: `cd app`
4. Install dependencies using PNPM: `pnpm i`
5. Run the application: `pnpx ts-node index.ts`
6. Observe that the Prisma client has not been generated

## Expected behavior

The Prisma client should be generated and the application should run without issues.

## Prisma information

Project set up accoring to [Start from scratch guide](https://www.prisma.io/docs/getting-started/setup-prisma/start-from-scratch-typescript-postgres).

## Environment & setup

- OS: Manjaro Linux x86_64
- Database: PostgreSQL 12
- Node.js version: v14.15.2
- Prisma version:

```
prisma               : 2.21.2
@prisma/client       : 2.21.2
Current platform     : debian-openssl-1.1.x
Query Engine         : query-engine e421996c87d5f3c8f7eeadd502d4ad402c89464d (at ../node_modules/.pnpm/@prisma+engines@2.21.0-36.e421996c87d5f3c8f7eeadd502d4ad402c89464d/node_modules/@prisma/engines/query-engine-debian-openssl-1.1.x)
Migration Engine     : migration-engine-cli e421996c87d5f3c8f7eeadd502d4ad402c89464d (at ../node_modules/.pnpm/@prisma+engines@2.21.0-36.e421996c87d5f3c8f7eeadd502d4ad402c89464d/node_modules/@prisma/engines/migration-engine-debian-openssl-1.1.x)
Introspection Engine : introspection-core e421996c87d5f3c8f7eeadd502d4ad402c89464d (at ../node_modules/.pnpm/@prisma+engines@2.21.0-36.e421996c87d5f3c8f7eeadd502d4ad402c89464d/node_modules/@prisma/engines/introspection-engine-debian-openssl-1.1.x)
Format Binary        : prisma-fmt e421996c87d5f3c8f7eeadd502d4ad402c89464d (at ../node_modules/.pnpm/@prisma+engines@2.21.0-36.e421996c87d5f3c8f7eeadd502d4ad402c89464d/node_modules/@prisma/engines/prisma-fmt-debian-openssl-1.1.x)
Default Engines Hash : e421996c87d5f3c8f7eeadd502d4ad402c89464d
Studio               : 0.371.0
```
