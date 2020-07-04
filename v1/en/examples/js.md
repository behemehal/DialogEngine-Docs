# [DialogEngine JavaScript SDK](https://github.com/behemehal/DialogEngine-JS)

`npm i dialogengine-js`

### Construct Assistant
```js
var assisant = new DialogEngineSDK('clientid', 'language');
```


### Construct Conversation
```js
var conversation = new assistant.Conversation('conversationid')
```

### Get specific fallback
```js
conversation.getFallback('fallbackName') -> Promise.<Response>
```

### Get welcome fallback
```js
conversation.welcomeFallback() -> Promise.<Response>
```

### Talk
```js
conversation.talk(message) -> Promise.<Response>
```
