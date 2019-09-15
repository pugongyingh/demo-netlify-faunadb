# Demo: Netlify and FaunaDB

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/mikaelvesavuori/demo-netlify-faunadb)

This is a super-simple demo of using FaunaDB with Netlify. There is a bigger, official demo at [https://github.com/netlify/netlify-faunadb-example](https://github.com/netlify/netlify-faunadb-example) but I wanted to go for something more minimal. It uses [faunadb-js-release](https://github.com/fauna/faunadb-js-release) and a completely plain-vanilla JS example.

A nice blog post also exists at [https://www.netlify.com/blog/2019/09/10/announcing-the-faunadb-add-on-for-netlify/](https://www.netlify.com/blog/2019/09/10/announcing-the-faunadb-add-on-for-netlify/) which forms a bit of the initial basis of this repo.

For this demo, we will generally follow the steps laid out in [https://docs.fauna.com/fauna/current/tutorials/crud](https://docs.fauna.com/fauna/current/tutorials/crud).

**Additional resources can be found at:**

- [FaunaDB Add-on for Netlify](https://docs.fauna.com/fauna/current/start/netlify)
- [Netlify documentation](https://www.netlify.com/docs/)
- [FaunaDB CRUD examples](https://docs.fauna.com/fauna/current/tutorials/crud_examples.html)

## Instructions

### Installation

- Install the Netlify CLI with `npm i netlify-cli -g` or `yarn global add netlify-cli`
- Inside of your project directory, run `netlify init`
- Add the FaunaDB add-on with `netlify addons:create fauna`
- Authenticate with `netlify addons:auth fauna`
- Get a [Cloud Key](https://app.fauna.com/keys)
- Set the Cloud Key (aka "secret") in `index.html` at `const secret = 'CHANGE THIS'`
