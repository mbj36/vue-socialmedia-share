# vue-socialmedia-share

> Vue component for social sharing

<img width="688" alt="screen shot 2018-05-30 at 4 46 44 pm" src="https://user-images.githubusercontent.com/9936881/40717210-2a117e2e-6429-11e8-8230-cc0b22094d96.png">

### vue-socialmedia-share is a vue component for sharing links to social networks

## Demo

[![Edit vue-socialmedia-share](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/kk0mqj11lv)

## Features

* No external script loading
* Opens a new share tab
* Share Button for:
  * [Facebook](https://github.com/mbj36/vue-socialmedia-share#facebook)
  * [Twitter](https://github.com/mbj36/vue-socialmedia-share#twitter)
  * [Reddit](https://github.com/mbj36/vue-socialmedia-share#reddit)
  * [LinkedIn](https://github.com/mbj36/vue-socialmedia-share#linkedin)
  * [Google +](https://github.com/mbj36/vue-socialmedia-share#google-)
  * [WhatsApp](https://github.com/mbj36/vue-socialmedia-share#whatsapp)
  * [Telegram](https://github.com/mbj36/vue-socialmedia-share#telegram)
  * [Email](https://github.com/mbj36/vue-socialmedia-share#email)
  * [Pinterest](https://github.com/mbj36/vue-socialmedia-share#pinterest)
* Social Media icons includes in the library
* Change the size of icons

## Installation

```
yarn add vue-socialmedia-share
```

or

```
npm install vue-socialmedia-share
```

# API

## Facebook

```js
import { Facebook } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Facebook
  }
};
```

#### Props

| Prop    | Data Type | Required | Description        |
| ------- | --------- | -------- | ------------------ |
| `url`   | String    | true     | URL to share.      |
| `scale` | String    |          | Size of icon (1-9) |

## Twitter

```js
import { Twitter } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Twitter
  }
};
```

| Prop    | Data Type | Required | Description              |
| ------- | --------- | -------- | ------------------------ |
| `url`   | String    | true     | URL to share.            |
| `scale` | String    |          | Size of icon(1-9)        |
| `title` | String    |          | Title of the shared page |

## LinkedIn

```js
import { Linkedin } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Linkedin
  }
};
```

| Prop    | Data Type | Required | Description       |
| ------- | --------- | -------- | ----------------- |
| `url`   | String    | true     | URL to share.     |
| `scale` | String    |          | Size of icon(1-9) |

## Reddit

```js
import { Reddit } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Reddit
  }
};
```

| Prop    | Data Type | Required | Description              |
| ------- | --------- | -------- | ------------------------ |
| `url`   | String    | true     | URL to share.            |
| `scale` | String    |          | Size of icon(1-9)        |
| `title` | String    |          | Title of the shared page |

## Telegram

```js
import { Telegram } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Telegram
  }
};
```

| Prop    | Data Type | Required | Description              |
| ------- | --------- | -------- | ------------------------ |
| `url`   | String    | true     | URL to share.            |
| `scale` | String    |          | Size of icon(1-9)        |
| `title` | String    |          | Title of the shared page |

## WhatsApp

```js
import { WhatsApp } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    WhatsApp
  }
};
```

| Prop    | Data Type | Required | Description              |
| ------- | --------- | -------- | ------------------------ |
| `url`   | String    | true     | URL to share.            |
| `scale` | String    |          | Size of icon(1-9)        |
| `title` | String    |          | Title of the shared page |

## Pinterest

```js
import { Pinterest } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Pinterest
  }
};
```

| Prop    | Data Type | Required | Description       |
| ------- | --------- | -------- | ----------------- |
| `url`   | String    | true     | URL to share.     |
| `scale` | String    |          | Size of icon(1-9) |

## Google +

```js
import { Google } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Google
  }
};
```

| Prop    | Data Type | Required | Description       |
| ------- | --------- | -------- | ----------------- |
| `url`   | String    | true     | URL to share.     |
| `scale` | String    |          | Size of icon(1-9) |

## Email

```javascript
import { Email } from 'vue-socialmedia-share';

// usage in local component

export default {
  components: {
    Email
  }
};
```

| Prop      | Data Type | Required | Description       |
| --------- | --------- | -------- | ----------------- |
| `url`     | String    | true     | URL to share.     |
| `scale`   | String    |          | Size of icon(1-9) |
| `subject` | String    |          | Subject of email  |
| `body`    | String    |          | Body of email     |

## Contributing Guide

1.  Fork it!
2.  Create your feature branch: `git checkout -b my-new-feature`
3.  Commit your changes: `git commit -am 'Add some feature'`
4.  Push to the branch: `git push origin my-new-feature`
5.  Submit a pull request :D

## Author

&#169; [Mohit Bajoria](https://mbj36.xyz)

## License

[MIT](https://github.com/mbj36/vue-socialmedia-share/blob/master/LICENSE)

Like it ? <img src="https://assets-cdn.github.com/images/icons/emoji/unicode/2b50.png?v8" height="20px" /> it
