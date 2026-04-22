# 2-22-2222

Source for [2-22-2222.xyz](https://2-22-2222.xyz) — time traveller story and ordinals collection.

## Stack (same as nft.xowlz.com)

NGINX serves `public/`; **`/api/*`** → Node on port **4012**. Express entry: `api-server.js`.

```bash
cp .env.example .env
npm install
npm run dev
```

```bash
sudo cp site-2-22-2222.service /etc/systemd/system/
sudo systemctl daemon-reload
sudo systemctl enable --now site-2-22-2222.service
sudo cp ../../nginx/2-22-2222.xyz.conf /etc/nginx/sites-available/2-22-2222.xyz.conf
sudo nginx -t && sudo systemctl reload nginx
```
