# cypress 笔记

[cypress - 中文文档](https://docs.cypress.io/zh-cn/guides/overview/why-cypress.html#)

### setCookie

`setCookie`会在每个`it`之后自动销毁，保证纯洁性，所以需要修改整个`describe`的`cookie`需要在`beforeEach`中使用。参考：https://docs.cypress.io/api/commands/clearcookies.html#Syntax

> Cypress automatically clears all cookies before each test to prevent state from being shared across tests. You shouldn’t need to use this command unless you’re using it to clear a specific cookie inside a single test.
