# Local AI chat in the browser

A ChatGPT-style chat that runs **100% in your browser**: the language model is downloaded once and runs on your own device with [WebLLM](https://github.com/mlc-ai/web-llm) and WebGPU, in a Web Worker. No server, no API key, and your messages never leave your computer.

## Files

- `index.html` — chat UI and model loading
- `worker.js` — Web Worker that hosts the model engine

## Run it

Serve the folder over HTTP (WebGPU needs a secure context; `localhost` works) and open it in a WebGPU-capable browser such as Chrome:

```bash
npx serve .
```

The first load downloads the model, which can take a while.
