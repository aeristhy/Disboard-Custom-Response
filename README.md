# Disboard-Custom-Response
Just a simple DISBOARD Custom Response.

# CopyPaste
```js
    if (message.embeds.length && message.author.username == 'DISBOARD' && message.embeds[ 0 ].description.indexOf('Bump done') > -1) {
        message.delete();
        return message.channel.send('Thank you for bumping! Make sure to leave us a review (link your DISBOARD server)');
    } else {
        if (message.embeds.length && message.author.username == 'DISBOARD' && message.embeds[ 0 ].description.indexOf('Please wait another') > -1) {
            message.delete();
            return message.channel.send('Bump is not ready yet');
        }
    }
```
