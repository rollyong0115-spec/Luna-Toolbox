# Luna Toolbox V1

A standalone responsive browser application. No build step or account required. 26 built-in utilities and a directory of 34 external GitHub projects.

## Run on Windows
Open index.html directly for basic utilities, or run `python -m http.server 8080` from this folder and open http://localhost:8080. HTTPS or localhost is needed for some microphone and cryptography features.

## Deploy on GitHub Pages
Create a new public repository named `Luna-Toolbox`. Upload the six files in this folder (not the folder itself). Settings → Pages → Deploy from a branch → main → / (root) → Save. Open the URL displayed by GitHub. For Android Chrome, use the browser menu → Add to Home screen / Install app when available. Do not add API keys or private files to the public repository.

## Limitations
- Built-in notes, tasks and budget persist in browser localStorage; not encrypted or synced. Export backup regularly. Different URLs have separate storage.
- PDF and QR tools fetch pinned third-party JavaScript libraries on demand and need internet when not already loaded in the page. File processing happens in the browser. A hosted version caches its app shell for offline loading; the external library is not cached by the service worker.
- Speech recognition depends on browser and provider, may send audio to provider, and may need internet. Filipino voice availability varies. Audio recorder requires permission. Closing the tool stops recording; use Stop & save to export first.
- Video preview and timestamp export only; no automatic highlight detection or video encoding in V1.
- GitHub library is a directory, not installed software. AI chat, PC automation, system-level monitoring and remote control require separately installed tools; no AI provider keys or native permissions included.
- Check README/license and official release instructions for each external project. Some external services or distributions may cost money.
