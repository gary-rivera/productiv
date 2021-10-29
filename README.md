<h1 align="center"> # Extra API 🧠 <h1/>

[![codecov](https://codecov.io/gh/ThingyThingInc/extra-api/branch/master/graph/badge.svg?token=1zQBpt6fkq)](https://codecov.io/gh/ThingyThingInc/extra-api)

## About

*The backend infracture to [Extra's Application](https://extra.app/).*

Associated Repos: 
- [extra-website ✨ ](https://github.com/ThingyThingInc/extra-website) - Extra's shiny new frontend application written in Vue


3rd Party Applications: 
- APTO ([Docs](https://docs.aptopayments.com/docs/overview/welcome/))
- Customer.io ([Docs](https://customer.io/docs/api/#tag/trackOverview))
- Datalinx ([Docs](https://datalinxllc.com/credit-reporting-software-system))
- Dwolla ([Docs](https://docs.dwolla.com/))
- Objection.js ([Docs](https://vincit.github.io/objection.js/guide/))
- Plaid ([Docs](https://plaid.com/docs/))
- Stripe ([Docs](https://stripe.com/docs/api))
- SentiLink ([Docs](https://www.sentilink.com/products/synthetic-fraud-scores))
- Sentry ([Docs](https://docs.sentry.io/platforms/node/guides/express/))
- Twilio ([Docs](https://www.twilio.com/docs))
  
## Setup 
### Installation

```bash
# clone repo
$ git clone https://github.com/ThingyThingInc/extra-api.git

# install dependencies
$ yarn install
```

### Development

```bash
$ yarn dev
```


## Usage/Examples

#### Get a user

```http
  GET v1/users/${user_id}
```

&nbsp;or

```http
  GET v1/users/me
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `user_id` | `string` | **Requires** a Bearer authorization token |

_Reference: https://github.com/ThingyThingInc/extra-api/blob/bfa63914c4e02eefc40b36c632fab205d8d18997/src/routes/users/index.ts#L63-L94_


#### Post a user

```http
  POST v1/users/
```

| Body | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `userData`      | `object` | **Requires** a Bearer authorization token |

_Reference: https://github.com/ThingyThingInc/extra-api/blob/bfa63914c4e02eefc40b36c632fab205d8d18997/src/routes/users/index.ts#L225-L235_

## CI

![Primary](https://github.com/ThingyThingInc/extra-api/workflows/Primary/badge.svg)
![Secondary](https://github.com/ThingyThingInc/extra-api/workflows/Secondary/badge.svg)

### Production

- `master` - deploys to prod (be careful)
- `fasttrack` - deploys to prod w/o unit testing or migrations (be extra careful)
- `migrations` - runs migrations in prod w/o deploying (maybe be careful)

### Sandbox

- `sandbox` - deploys to sandbox w/ unit testing and migrations (have at it)
### Technology Stacks

- [TypeScript](https://www.typescriptlang.org/docs/) - The language our API is written in.   
- [Node v.16.7.0](https://nodejs.org/en/docs/) - Server-side client
- [Express v4.16.4](http://expressjs.com/en/api.html) - Application server framework 
- [Objection.js](https://vincit.github.io/objection.js/guide/getting-started.html) - Extra's ORM of choice with knex.js under the hood. 
- [MySQL](https://dev.mysql.com/doc/refman/8.0/en/) - Relational Database Manager software(RDBMS)
## Roadmap

- https://linear.app/extra/team/ENG/active

## Appendix
- Notion Links:
  - [Dev](https://www.notion.so/getextra/Dev-8c47a107fb9a4fd297a40ad0733a8c3c)
  - [Extra Engineering Manual](https://www.notion.so/getextra/The-Extra-Manual-59db215e7c4548cfac55b550d2ebe409)
  - [Specs](https://www.notion.so/getextra/46628d86378a4f918940e206feca603e?v=ed78740c161b458383051cb4e8e9f6af)
- [API Walkthrough](https://drive.google.com/file/d/1xBVmi5RHms5ZTHNyI6YS_uKWYFZTNBpk/view)
