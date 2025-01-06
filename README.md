# Nexus.js

Une bibliothèque Discord moderne et puissante pour Node.js.

## Installation

```bash
npm install nexus.js
```

## Caractéristiques

- 🚀 API moderne et intuitive
- ⚡ Performance optimisée
- 🛡️ Typesafe avec support TypeScript
- 🔧 Facilement extensible
- 📦 Zéro dépendance inutile

## Utilisation rapide

```javascript
const { Client, Events } = require('nexus.js');

const client = new Client({
    intents: ['GUILDS', 'GUILD_MESSAGES']
});

client.on(Events.MESSAGE_CREATE, message => {
    if (message.content === '!ping') {
        message.reply('Pong!');
    }
});

client.login('your-token-here');
```

## Tests

Pour exécuter les tests, vous devez d'abord configurer un bot de test :

1. Créez un nouveau bot sur le [Portail Développeur Discord](https://discord.com/developers/applications)
2. Copiez le token du bot
3. Créez un fichier `.env` à la racine du projet avec le contenu suivant :
   ```
   DISCORD_TOKEN=your-bot-token-here
   ```
4. Exécutez les tests :
   ```bash
   npm test
   ```

## Documentation

La documentation complète est disponible [ici](lien-vers-la-documentation).

## Contribution

Les contributions sont les bienvenues ! Veuillez lire le guide de contribution avant de soumettre une pull request.

## Licence

MIT

## Support

- [Serveur Discord](https://discord.gg/nexusjs)
- [GitHub Issues](https://github.com/yourusername/nexus.js/issues)

## Crédits

Créé avec ❤️ par [Henelio]
