# FoodieHub — Mock REST API

A JSON Server backend for the [FoodieHub React application](https://github.com/sangeethareddy9/foodiehub-frontend). It exposes the collections in `db.json` as REST resources for frontend practice.

**Stack:** Node.js and JSON Server 0.17.

## Run locally

```bash
git clone https://github.com/sangeethareddy9/foodiehub-backend.git
cd foodiehub-backend
npm ci
npm start
```

The server listens on `http://localhost:3000` by default. Set the `PORT` environment variable to use another port.

## Files

| File | Purpose |
| --- | --- |
| [server.js](server.js) | Creates the JSON Server instance, default middleware and router |
| [db.json](db.json) | File-backed resource data |
| [package.json](package.json) | Dependencies and start command |
| [package-lock.json](package-lock.json) | Dependency lockfile |

## Frontend connection

In the frontend's `src/services/api.js`, set the Axios `baseURL` to the address of this server.

JSON Server supplies standard collection and item routes, such as `GET /users` for the user collection used by the frontend.

## Demo scope

This is a mock API for learning CRUD and frontend integration. It does not implement secure authentication, authorization or password hashing. Use fictional test data only.

## Author

[Sangeetha Chirla](https://github.com/sangeethareddy9)
