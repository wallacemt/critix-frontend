# Umami

The web frontend loads the Umami tracker when `NEXT_PUBLIC_UMAMI_WEBSITE_ID` is set. Create a separate Umami website for Critix, then configure that ID as a GitHub Actions repository variable with the same name so Docker builds include it. For local builds, put the ID in `.env.local`.

The tracker uses `https://analytics.wallacedev.com.br/script.js`, accepts only `critix.app` and `critix.wallacedev.com.br`, respects Do Not Track, and omits query strings and URL hashes from pageviews.
