# ![LOGO](logo.png) Service User **flow**ground Connector

## Description

A generated **flow**ground connector for the Service User API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/serviceuser/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:57+03:00

## API Description

Enables services that service consumers want to use on Google Cloud Platform, lists the available or enabled services, or disables services that service consumers no longer use.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Search available services.<br/>
> <br/>
> When no filter is specified, returns all accessible services. For<br/>
> authenticated users, also returns all services the calling user has<br/>
> "servicemanagement.services.bind" permission for.

*Tags:* `services`

#### Input Parameters
* `pageSize` - _optional_ - Requested size of the next page of data.
* `pageToken` - _optional_ - Token identifying which result to start with; returned by a previous list
call.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `bearer_token` - _optional_ - OAuth bearer token.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `pp` - _optional_ - Pretty-print response.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Disable a service so it can no longer be used with a<br/>
> project. This prevents unintended usage that may cause unexpected billing<br/>
> charges or security leaks.<br/>
> <br/>
> Operation<response: google.protobuf.Empty>

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Name of the consumer and the service to disable for that consumer.

The Service User implementation accepts the following forms for consumer:
- "project:<project_id>"

A valid path would be:
- /v1/projects/my-project/services/servicemanagement.googleapis.com:disable
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `bearer_token` - _optional_ - OAuth bearer token.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `pp` - _optional_ - Pretty-print response.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Enable a service so it can be used with a project.<br/>
> See [Cloud Auth Guide](https://cloud.google.com/docs/authentication) for<br/>
> more information.<br/>
> <br/>
> Operation<response: google.protobuf.Empty>

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - Name of the consumer and the service to enable for that consumer.

A valid path would be:
- /v1/projects/my-project/services/servicemanagement.googleapis.com:enable
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `bearer_token` - _optional_ - OAuth bearer token.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `pp` - _optional_ - Pretty-print response.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### List enabled services for the specified consumer.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - Requested size of the next page of data.
* `pageToken` - _optional_ - Token identifying which result to start with; returned by a previous list
call.
* `parent` - _required_ - List enabled services for the specified parent.

An example valid parent would be:
- projects/my-project
* `bearer_token` - _optional_ - OAuth bearer token.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `pp` - _optional_ - Pretty-print response.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-serviceuser-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
