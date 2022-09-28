## Dependencies

- express
- cors

## Dev Dependencies

### Node

- nodemon
- typescript
- @types/node
- rimraf

### Framework

- @types/express

### Test

- jest
- ts-jest
- @types/jest
- supertest
- @types/supertest

### Code style and Lint

- husky
- eslint
- @typescript-eslint/eslint-plugin
- @typescript-eslint/parser
- prettier
- eslint-config-prettier
- eslint-plugin-prettier

### help migrations

npm run typeorm -- -help

### init migrations

npm run typeorm:migrate init -- -d src/migrations

### run migrations pendings

npm run typeorm:run

### When get migrations test db

put cross-env NODE_ENV=test in package.json ahead of typeorm:migrate and typeorm:run

### Creating the initial data for superadmin

1. npm run seed:config
2. npm run seed:run

### well practice when change or add field to table in database

npm run typeorm:migrate added_column_hola_to_users -- -d src/migrations

### run test only one file example in windows

npm test src/tests/cities/cities.service.test.ts
