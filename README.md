# local-file-tunnel

Create temporary local file server with ngrok tunnel.

If you don't set an `NGROK_AUTHTOKEN` in a `.env` file, you will be cursed with the ngrok session timeout.

## Ngrok

As this runs in a Docker container, the typing ngrok UI you're used to isn't available. You must use the web view at http://localhost:4040

## Copy Files

You have to copy files you want to share to the running container:

```
docker compose cp ~/Pictures/test.png nginx:/usr/share/nginx/html
```
