---
name: Ping an organization webhook
example: octokit.rest.orgs.pingWebhook({ org, hook_id })
route: POST /orgs/{org}/hooks/{hook_id}/pings
scope: orgs
type: API method
---

# Ping an organization webhook

This will trigger a [ping event](https://docs.github.com/webhooks/#ping-event) to be sent to the hook.

```js
octokit.rest.orgs.pingWebhook({
  org,
  hook_id,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>org</td><td>yes</td><td>

The organization name. The name is not case sensitive.

</td></tr>
<tr><td>hook_id</td><td>yes</td><td>

The unique identifier of the hook.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/reference/orgs#ping-an-organization-webhook).
