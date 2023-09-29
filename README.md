# kli-cm-api

> Disclaimer: This is a fork of [kril-cm-api](https://github.com/krilbert/kril-cm-api) that is currently WIP to fix bugs and update it to Campaign Monitor API v3.3

This library uses Campaign Monitor API v3.3

## Getting started

```shell
npm i kli-cm-api
```

usage

```javascript
import { Transactional } from 'kli-cm-api'

try {
  const apiKey = 'xxx='
  const transactional = new Transactional({ apiKey })
  const data = await transactional.getStatistics()
  console.log(data)
} catch (err) {
  console.log(err)
}
```

> If you are using javascript don't forget to add @ts-check at the top of your file for a better experience

## Modules

[Campaign Monitor API](https://www.campaignmonitor.com/api) documentation.

| Module        | Description                                                                                                             |
| ------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Account       | Gives you access to core account information.                                                                           |
| Campaign     | Covers all the campaign related functionality including creating draft campaigns, selecting recipients and sending.     |
| Client       | Contains all the functionality you need to manage the clients in your account                                           |
| Journey      | Covers read-only journey functionality including viewing all journeys, journey summary, and detailed journey reporting. |
| List         | Covers all your list management needs.                                                                                  |
| Segment      | Segments allow you to create targeted sub-groups of subscribers based on conditions you set.                            |
| Subscriber   | Everything you need to work with subscribers in your account.                                                           |
| Template     | Templates make it easy for your clients to send great looking emails by just adding their own content.                  |
| Transactional | Transactional emails are triggered by your own site or app, typically in response to a user's action                    |
