## For database we use neondb. to connect to db we use prisma

## npm i -D prisma

## npx prisma init - which helps to initialize prisma inside our project.

/\*
Next steps:

1. Set the DATABASE_URL in the .env file to point to your existing database. If your database has no tables yet, re
   ad https://pris.ly/d/getting-started
2. Set the provider of the datasource block in schema.prisma to match your database: postgresql, mysql, sqlite, sql
   server, mongodb or cockroachdb.
3. Run prisma db pull to turn your database schema into a Prisma schema.
4. Run prisma generate to generate the Prisma Client. You can then start querying your database.
5. Tip: Explore how you can extend the ORM with scalable connection pooling, global caching, and real-time database
   events. Read: https://pris.ly/cli/beyond-orm
   \*/

![ Data base table info](image.png)-- here we can know how the table structure is created.

## Now we will see how the table structure can be created in the database via nextjs.

1. Navigate to schema.prisma file and there we will create the schema.
2. Now we need to create these tables in neondb.
3. npx prisma generate. -- it will create tables in the database.
4. npx prisma migrate dev -- this will show what and queries it has been created while creating the tables.
5. Now inside lib folder we do create a prisma.js file which will help us to query our database.

## Now for creating organizations we have that feature in clerk.

1. navigate to ur project in the header section we do have organization.
2. click on it and enable the organization.
3. in the left side panel we do have link for path. in this we specify sign-in and sign-up which will be helpful for sending emails links.
