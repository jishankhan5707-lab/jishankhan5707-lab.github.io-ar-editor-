# Orbit AI Chat

A small, responsive AI chat interface that can be hosted as a static website, including on GitHub Pages.

## Run it

Open `index.html` in a browser, or publish the repository with GitHub Pages. Click **API key** and enter an [OpenAI API key](https://platform.openai.com/api-keys). The app calls OpenAI's Chat Completions API using `gpt-4o-mini`.

## Important security note

This is a static, browser-only demo. The key is held in `sessionStorage` for the current browser tab and sent from the browser directly to OpenAI. Anyone with access to the browser's developer tools can inspect it, and browser-based requests may be subject to cross-origin restrictions. Do not use this on a shared device, commit a real API key, or treat it as a production-safe setup. For a public production app, put the API request behind a server or serverless function and store the key in that service's secret environment variables; add authentication and rate limits as appropriate.

Chat history is kept in memory only and is cleared when you click **New chat** or reload the page.
