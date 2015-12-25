# Chrome Offline page "T-Rex Runner" game bot

![TRex](http://i.imgur.com/9oO7aQ9.gif)

### Try it out

Copy the minified source code, disconnect from the Internet and paste it to the Console in Chrome Dev tools.

```javascript
function TrexRunnerBot(){function n(){if(Runner&&Runner().horizon.obstacles[0]){var n=Runner().horizon.obstacles[0];e(n)&&o(n)&&r(n)}}function e(n){return 50!==n.yPos}function o(n){return n.xPos<=18*Runner().currentSpeed}function r(n){u(n)?t():c(n)}function u(n){return 75===n.yPos}function t(){Runner().onKeyDown(R),setTimeout(function(){Runner().onKeyUp(R)},500)}function c(n){i(n)?f():Runner().onKeyDown(s)}function i(n){var e=Runner().horizon.obstacles[1];return e&&e.xPos-n.xPos<=42*Runner().currentSpeed}function f(){Runner().onKeyDown(s),Runner().onKeyUp(s)}var s={keyCode:38},R={keyCode:40,preventDefault:function(){}};return{conquerTheGame:n}}var bot=TrexRunnerBot(),botInterval=setInterval(bot.conquerTheGame,2);
```

## License

[MIT](//github.com/ukupat/trex-runner-bot/blob/master/LICENSE)
