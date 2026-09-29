# SEC Studio Cloud

## Run
1. Install Node.js 20+ and FFmpeg.
2. Copy `.env.example` to `.env`.
3. Add Google/GitHub OAuth credentials if you want OAuth login.
4. Run `npm install`
5. Run `npm start`
6. Open http://localhost:3000

## Real now
- Server-side FFmpeg H.264/AAC rendering
- 1080p and 4K output selection
- Google/GitHub OAuth implementation
- Sessions and profile UI
- Video upload/preview
- AI endpoint architecture

## Requires model provider
AI captions, background removal, and object tracking need an actual inference model/API. The endpoints intentionally return 501 until one is connected; they do not fake AI output.

## H.265
Add `libx265` to the FFmpeg render pipeline only on a server whose FFmpeg build includes it and where your distribution/codec requirements permit it.
