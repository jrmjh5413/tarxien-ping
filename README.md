# tarxien-ping

Fetches the hosted [Tarxien](https://github.com/jrmjh5413/tarxien) instance
every 5 minutes so Render's free tier never spins it down — a sleeping server
can't send push reminders. The instance URL lives in the `RENDER_URL` repo
secret; without it the workflow exits quietly. The app itself is
password-gated, so the pinger only ever sees the login shell.
