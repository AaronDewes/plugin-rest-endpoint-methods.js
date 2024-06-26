---
name: Delete a self-hosted runner from an organization
example: octokit.rest.actions.deleteSelfHostedRunnerFromOrg({ org, runner_id })
route: DELETE /orgs/{org}/actions/runners/{runner_id}
scope: actions
type: API method
---

# Delete a self-hosted runner from an organization

Forces the removal of a self-hosted runner from an organization. You can use this endpoint to completely remove the runner when the machine you were using no longer exists.

Authenticated users must have admin access to the organization to use this endpoint.

OAuth tokens and personal access tokens (classic) need the`admin:org` scope to use this endpoint. If the repository is private, OAuth tokens and personal access tokens (classic) need the `repo` scope to use this endpoint.

```js
octokit.rest.actions.deleteSelfHostedRunnerFromOrg({
  org,
  runner_id,
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
<tr><td>runner_id</td><td>yes</td><td>

Unique identifier of the self-hosted runner.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/actions/self-hosted-runners#delete-a-self-hosted-runner-from-an-organization).
