# TalkitWeb
Developed TalkItWeb, a real-time web chat application that enables instant messaging between users through a responsive and intuitive interface. Implemented efficient backend communication and real-time message handling to ensure smooth and scalable user interactions.

## Deployment readiness

This repository is configured to run as a single Node service that serves the backend API and (in production) the built frontend static files.

### Prerequisites

- Node.js 20+
- npm 10+

### Environment variables

Create a `.env` file in `backend/` based on `.env.example`.

Required variables:

- `PORT` (optional, defaults to `3000`)
- `NODE_ENV` (`production` in deployment)

### Install and build

From repository root:

```bash
npm install
npm run build
```

### Start in production

From repository root:

```bash
npm start
```

### Health check

After start, verify:

`GET /health` returns HTTP 200 with `{ "status": "ok" }`.
