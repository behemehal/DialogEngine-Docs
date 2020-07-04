# [DialogEngine JavaScript SDK](https://github.com/behemehal/DialogEngine-JS)

### Construct Assistant
```js
var assisant = new DialogEngineSDK('clientid', 'language');
```


### Construct Conversation
```js
var conversation = new assistant.Conversation('conversationid')
```

### Get specific intent
```js
conversation.getIntent('intentName') -> Promise.<Response>
```


### Get welcome intent
```js
conversation.welcomeIntent() -> Promise.<Response>
```

### Talk
```js
conversation.talk(message) -> Promise.<Response>
```