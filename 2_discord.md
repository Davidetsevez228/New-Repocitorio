# Documentació del Bot de Discord

![Logotip de Discord](https://assets-global.website-files.com/6257adef93867e50d84d30e2/636e0a6a49cf127bf92de1e2_icon_clyde_blurple_RGB.png)

Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord](https://discord.com/developers/applications).

Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`

```javascript
client.on('messageCreate', message => {
    if (message.content === 'ping') {
        message.reply('pong!');
    }
});
