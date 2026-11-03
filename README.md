# inventory-sync-service

Syncs on-hand inventory from the store POS feed into the central inventory API
and exports nightly snapshots to S3.

## Setup
1. Copy `.env` and set `APP_ENV`
2. AWS creds are in `.aws/credentials` (profile `inventory-sync-prod`)
3. Ops dashboard status page: see `OPS_WEBHOOK_URL` in `.env`

## Run
python sync.py --profile inventory-sync-prod
