# emoji-armor
[![NPM](https://nodei.co/npm/emoji-armor.png)](https://nodei.co/npm/emoji-armor/)


```js
var armor = require('emoji-armor')
var fs = require('fs')

var encode = armor('😊🔒')

fs.createReadStream('test.js')
  .pipe(encode)
  .pipe(process.stdout)
```

This prints something like this to the console:
```
💜💜💜💜💜💜🔜😊🔒💜💜💜💜💜💜💜
🎲🌳🍀🔋🌳🍀👣🔦🍀🔋💡🔋🍀🐬🏈🐸
👂🍀🐬🎂👙🐗⛵️👙🃏⚓️🎲🌳🍀🔋🍩🍤
🔋💡🔋🍀🐬🏈🐸👂🍀🐬🎂👙🍩🍤👙🃏
⚓️⚓️🎲🌳🍀🔋🐬🔥🐕🔦💵🐬🔋💡🔋🌳
🍀👣🔦🍀🎂👙🎩🍄🔬🎃🎩🍄🍁🔍👙🃏
⚓️🎲🌳🍀🔋💵🐬🐕🔦💵🐬🔋💡🔋🌳🍀
👣🔦🍀🐗💵🐬🐕🔦💵🐬🎂🃏⚓️⚓️🍩🍤
🐗🐕🍀🐬🌳🍟🐬💻🐬🌳💵🎊🍟🍀🐬🌳
👣🎂👙🍟🐬🍤🍟🐗🌍🍤👙🃏⚓️🔋🔋🐗
💾👂💾🐬🎂🐬🔥🐕🔦💵🐬🃏⚓️🔋🔋⛵️
⛵️🔋🐗💾👂💾🐬🎂💵🐬🐕🔦💵🐬🃏⚓️
🔋🔋🐗💾👂💾🐬🎂💾🍀🔦🐕🐬🍤🍤🐗
🍤🍟💵🔦🐸🍟🃏⚓️🔋🔋
💜💜💜💜💜💜🔚😊🔒💜💜💜💜💜💜💜
```

## armor(name)

alias for armor.encode(name)

## armor.encode(name)

returns a transform stream for encoding to emoji

## armor.decode(name)

transform stream for decoding from emoji armor
