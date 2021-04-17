# `@shop0/shop0-api`

<!-- ![Build Status]() -->

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE.md)
[![npm version](https://badge.fury.io/js/%40shop0%2Fshop0-api.svg)](https://badge.fury.io/js/%40shop0%2Fshop0-api)

支持 TypeScript/JavaScript [shop0](https://www.shop0.com) 应用访问 [shop0 Admin API](https://shop0.dev/docs/admin-api), by making it easier to perform the following actions:

- Creating [online](https://shop0.dev/concepts/about-apis/authentication#online-access) or [offline](https://shop0.dev/concepts/about-apis/authentication#offline-access) access tokens for the Admin API via OAuth
- 调用 [REST API](https://shop0.dev/docs/admin-api/rest/reference)
- 调用 [GraphQL API](https://shop0.dev/docs/admin-api/graphql/reference)
- 注册/处理 webhooks

此 SDK 提供给 Node.js 后端应用使用, 不依赖特殊的框架，所以你可以在任何技术栈中使用.

# Requirements

To follow these usage guides, you will need to:

- have a basic understanding of [Node.js](https://nodejs.org)
- 拥有 shop0 开发者账号和可测试店铺
- _OR_ 针对店铺创建私有 APP
- have a private or custom app already set up in your test store or partner account
- 采用 [ngrok](https://ngrok.com), 可以在你本机创建一个应用的反向代理安全通道
- add the `ngrok` URL and the appropriate redirect for your OAuth callback route to your app settings
- have [yarn](https://yarnpkg.com) installed

<!-- Make sure this section is in sync with docs/README.md -->

# Getting started

You can follow our [getting started guide](docs/), which will provide instructions on how to create an app using plain Node.js code, or the [Express](https://expressjs.com/) framework. Both examples are written in Typescript.

- [Getting started](docs/getting_started.md)
  - [Install dependencies](docs/getting_started.md#install-dependencies)
  - [Set up base files](docs/getting_started.md#set-up-base-files)
  - [Set up environment](docs/getting_started.md#set-up-environment)
  - [Set up Context](docs/getting_started.md#set-up-context)
  - [Running your app](docs/getting_started.md#running-your-app)
- [Performing OAuth](docs/usage/oauth.md)
  - [Add a route to start OAuth](docs/usage/oauth.md#add-a-route-to-start-oauth)
  - [Add your OAuth callback route](docs/usage/oauth.md#add-your-oauth-callback-route)
  - [Fetching sessions](docs/usage/oauth.md#fetching-sessions)
  - [Detecting scope changes](docs/usage/oauth.md#detecting-scope-changes)
- [Make a REST API call](docs/usage/rest.md)
- [Make a GraphQL API call](docs/usage/graphql.md)
- [Webhooks](docs/usage/webhooks.md)
  - [Register a Webhook](docs/usage/webhooks.md#register-a-webhook)
  - [Process a Webhook](docs/usage/webhooks.md#process-a-webhook)
- [Known issues and caveats](docs/issues.md)
  - [Notes on session handling](docs/issues.md#notes-on-session-handling)
