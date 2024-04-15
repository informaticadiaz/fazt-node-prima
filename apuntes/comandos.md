# Comandos

Este documento pretende ser una lista de comandos necesarios para desarrollar el proyecto.

Inicializamos un proyecto

```bash
pnpm init
```

Instalamos Prisma

```bash
pnpm i prisma -D
```

Inicializa Prisma

```bash
npx prisma init
```

Ejecuta la migración

```bash
npx prisma migrate dev
```

## Anotaciones

-D para instalar como dependencia de desarrollo

Cuando se ejecuta `npx prisma init` crea un archivo `prisma/schema.prisma` en el directorio root, el archivo `prisma/schema.prisma` es el que se encarga de definir la base de datos.

este es el mensaje que da la consola cuando se ejecuta npx prisma init

npx prisma init

✔ Your Prisma schema was created at prisma/schema.prisma
  You can now open it in your favorite editor.

Next steps:

1. Set the DATABASE_URL in the .env file to point to your existing database. If your database has no tables yet, read `https://pris.ly/d/getting-started`
2. Set the provider of the datasource block in schema.prisma to match your database: postgresql, mysql, sqlite, sqlserver, mongodb or cockroachdb.
3. Run prisma db pull to turn your database schema into a Prisma schema.
4. Run prisma generate to generate the Prisma Client. You can then start querying your database.

More information in our documentation:
`https://pris.ly/d/getting-started`

┌────────────────────────────────────────────────────────────────┐
│  Developing real-time features?                                │
│  Prisma Pulse lets you respond instantly to database changes.  │
│  `https://pris.ly/cli/`pulse                                     │
└──────────────────────────────────────────

### Migracion

Las migraciones en las bases de datos se utilizan para crear y actualizar la base de datos.
Cuando ejecutemos `npx prisma migrate dev` se crea una carpeta dentro del directorio prisma que contiene la migración de la base de datos.
