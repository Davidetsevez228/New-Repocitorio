# Documentación del Bot de Discord

![Logotipo de Discord](https://assets-global.website-files.com/6257adef93867e50d84d30e2/636e0a6a49cf127bf92de1e2_icon_clyde_blurple_RGB.png)

Puedes registrar tu aplicación en el [Portal de Desarrolladores de Discord](https://discord.com/developers/applications).

Para hacer que el bot responda, escuchamos el evento `messageCreate` y utilizamos el método `message.reply()`

```javascript
client.on('messageCreate', message => {
    if (message.content === 'ping') {
        message.reply('pong!');
    }
});
