# Grand Tournoi — site officiel

Version premium responsive avec compteur Discord et inscription via webhook côté serveur.

## Déploiement gratuit
Cloudflare Workers :
1. `npm install -g wrangler`
2. `wrangler login`
3. `wrangler secret put DISCORD_WEBHOOK_URL`
4. `wrangler deploy`

Le webhook doit être stocké comme secret. Le webhook fourni dans la conversation est exposé : régénère-le dans Discord avant production.

## Connexion Discord
OAuth2 nécessite une application Discord avec Client ID + Client Secret. Le secret ne doit jamais être placé dans `public/`.
