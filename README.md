# CINEVA — website prototype

CINEVA is a colorful, welcoming creative studio concept for cinematic AI images and films.

## Run locally

- Install Node.js 20 or newer.
- Run `npm install`.
- Run `npm run dev`.
- Visit `http://localhost:3000`.

## What's built

- Responsive landing page and studio layout.
- Interactive prompt field, visual style and aspect-ratio controls.
- Session-only creative history.
- API route skeleton for a future server-side image-model integration.
- Environment-variable template.

## Not connected yet

- Real image generation: requires choosing a model/provider, implementing its adapter, and configuring secure server credentials.
- Authentication and durable user accounts.
- Persistent cloud gallery and exports.
- Production GPU hosting, queues, rate limits, moderation, and cost controls.

The current Create Image action is a front-end prototype. It does not generate an AI image yet.

## Next steps

1. Choose an image model and verify its license permits the intended hosted service.
2. Implement the provider adapter in `app/api/generate/route.ts`.
3. Add Supabase Auth and database/storage policies.
4. Add a durable job queue, GPU hosting, moderation, and usage limits.
5. Deploy to a hosting provider and connect a domain.

Never put provider secrets in client-side code.
