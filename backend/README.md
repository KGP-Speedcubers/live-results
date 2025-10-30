# Backend

## Running Locally

1. Update your [`.env`](./.env)
    1. Add `JWT_SECRET`, you can generate one randomly with 

    ```bash
    node -e "console.log(require('crypto').randomBytes(32).toString('hex'))"
    ```

    2. Add `ADMIN_PASSWORD`, this is the password used to access admin dashboard

2. Run backend

```bash
npm i
npm run start
```

## Running with Docker

Just update the `.env` file as above
