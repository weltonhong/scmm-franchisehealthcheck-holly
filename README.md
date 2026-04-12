# SCMM Franchise Health Check

Streamlit web app for running franchise home care online health checks at trade shows.

**Franchise version differences from the standard health check:**
- No website audit (franchise websites are corporate-built)
- No overall letter grade (individual section grades only)
- CTA routes to Vickey Lopez (Vickey.Lopez@RingRingMarketing.com)

## Deployment

Deployed on Streamlit Cloud at: `scmm-franchisehealthcheck-vickey.streamlit.app`

**Main file path:** `my-skills/franchise-tradeshow-healthcheck-homecare/webapp/app.py`

**Required Streamlit Cloud secrets** (TOML format in App Settings):
```toml
GOOGLE_API_KEY = "your-key"
SCRAPINGBEE_API_KEY = "your-key"
```

## Local Development

```bash
pip install -r my-skills/franchise-tradeshow-healthcheck-homecare/webapp/requirements.txt
streamlit run my-skills/franchise-tradeshow-healthcheck-homecare/webapp/app.py
```

## Sync Workflow

The canonical source is `my-powerhouse/my-skills/franchise-tradeshow-healthcheck-homecare/`.
After editing there, copy changed files to this repo at the same relative paths, then commit and push. Streamlit Cloud auto-redeploys within ~30s of a push.
