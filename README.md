# Anant 1.0 — Frontend

## Setup

No build tools needed. This is a single HTML file with inline CSS and JS.

### 1. Configure API URL

Open `index.html` and change the API URL at the top of the `<script>` section:

```javascript
const API_URL = "http://localhost:8000";
```

For ngrok tunneling:
```javascript
const API_URL = "https://your-tunnel.ngrok-free.dev";
```

### 2. Start the API backend

```bash
cd ~/Downloads/neural-ai/anant-finetune
source anant-env/bin/activate
PYTHONPATH=. python run_api.py
```

### 3. Open the frontend

Simply open in a browser:
```bash
open frontend/index.html
```

Or serve with any static server:
```bash
python3 -m http.server 3000 -d frontend
# Then open http://localhost:3000
```

## Features

- JWT authentication (signup/login)
- Real-time chat with Anant AI
- Collapsible thinking blocks
- Markdown rendering in responses
- Memory graph (3D interactive)
- Profile viewer
- Emotion trajectory
- Pattern discovery
- Memory statistics
- Dream cycle trigger
- Message feedback (thumbs up/down)
- Mobile responsive
- Keyboard shortcuts (Enter to send, Escape to close panels)
