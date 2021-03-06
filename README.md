[![Build Status](https://travis-ci.org/telemark/micro-universal-status.svg?branch=master)](https://travis-ci.org/telemark/micro-universal-status)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)
[![Greenkeeper badge](https://badges.greenkeeper.io/telemark/micro-universal-status.svg)](https://greenkeeper.io/)

# micro-universal-status

Pull stats from service

## API

GET/POST 
- **url** for status service
- **fields** for status
- **title** for html

### **/raw**

Returns json of unformatted data.

#### GET

```bash
$ curl https://universal.status.micro.t-fk.no/raw?url=<url>&fields=field1|field2|field3&title=yay
```

### POST

```JavaScript
{
  url: '<url>',
  fields: [
    'field1',
    'field2',
    'field3'
  ],
  title: 'yay'
}
```


### **/json**

Returns json of formatted data.

#### GET

```bash
$ curl https://universal.status.micro.t-fk.no/json?url=<url>&fields=field1|field2|field3&title=yay
```

### POST

```JavaScript
{
  url: '<url>',
  fields: [
    'field1',
    'field2',
    'field3'
  ],
  title: 'yay'
}
```

### **/html**

Renders formatted data to html. 

#### GET

```bash
$ curl https://universal.status.micro.t-fk.no/html?url=<url>&fields=field1|field2|field3&title=yay
```

### POST

```JavaScript
{
  url: '<url>',
  fields: [
    'field1',
    'field2',
    'field3'
  ],
  title: 'yay'
}
```

## License

[MIT](LICENSE)

![micro-universal-status](https://robots.kebabstudios.party/micro-universal-status.png "Robohash image of micro-universal-status")
