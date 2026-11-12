# Monster Hunter Wilds Field Relay

The field-report form posts JSON directly to the Cloudflare Worker configured in `index.html`. Update `WORKER_URL` there to your deployed Worker URL before publishing if the URL in the sample does not match your Worker.

The form sends `name`, `email`, `message`, and a hidden `website` honeypot field. The Worker should accept JSON POST requests and handle CORS for the domain hosting this page.