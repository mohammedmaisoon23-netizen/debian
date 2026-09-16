# HyperVM Render Console (Native Python Runtime)

This project runs on Render's native **Python 3** runtime without requiring Docker.

## Render Configuration Settings

When creating or configuring your Web Service on Render:
- **Runtime:** `Python 3`
- **Build Command:** `pip install -r requirements.txt`
- **Start Command:** `uvicorn server:app --host 0.0.0.0 --port $PORT`

## Environment Variables
Add the following secret variable in your Render dashboard under the **Environment** tab:
- `CONSOLE_TOKEN` = `your-secure-random-token-here`
