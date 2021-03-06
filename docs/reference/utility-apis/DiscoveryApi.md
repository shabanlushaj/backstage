# DiscoveryApi

The DiscoveryApi type is defined at
[packages/core-api/src/apis/definitions/DiscoveryApi.ts:30](https://github.com/spotify/backstage/blob/82d329555c16af46db9b4e5cd2f44a3cc006a52e/packages/core-api/src/apis/definitions/DiscoveryApi.ts#L30).

The following Utility API implements this type:
[discoveryApiRef](./README.md#discovery)

## Members

### getBaseUrl()

Returns the HTTP base backend URL for a given plugin, without a trailing slash.

This method must always be called just before making a request. as opposed to
fetching the URL when constructing an API client. That is to ensure that more
flexible routing patterns can be supported.

For example, asking for the URL for `auth` may return something like
`https://backstage.example.com/api/auth`

<pre>
getBaseUrl(pluginId: string): Promise&lt;string&gt;
</pre>
