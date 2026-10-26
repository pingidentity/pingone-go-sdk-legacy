# PingOne Administration GO SDK

The PingOne GO SDK provides a set of functions and stucts that help with interacting with the PingOne public cloud API.

The code is intended to be delivered as a sample, until an official GO SDK is released from Ping Identity.  As such, the code is highly likely to change significantly between releases. 

Code for each service is generated with the help of the [OpenAPI Generator](https://openapi-generator.tech/).

## Packages

The SDK provides a core package, and a package per PingOne service, each with their own directory off the root of the project:

* **authorize** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/authorize) - for the PingOne Authorize service
* **credentials** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/credentials) - for the PingOne Credentials service, part of PingOne Neo
* **management** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/management) - for the PingOne platform common and SSO services
* **mfa** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/mfa) - for the PingOne MFA service
* **risk** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/risk) - for the PingOne Protect service
* **verify** - [Documentation](https://pkg.go.dev/github.com/pingidentity/pingone-go-sdk-legacy/verify) - for the PingOne Verify service, part of PingOne Neo

## Getting Started

The client can be invoked using the following syntax:

```go

...

import (
	"context"

	"github.com/pingidentity/pingone-go-sdk-legacy/pingone"
)

...

config := &pingone.Config{
	ClientID:      clientId,
	ClientSecret:  clientSecret,
	EnvironmentID: environmentId,
	AccessToken:   accessToken,
	RegionCode:    regionCode,
}

client, err := config.APIClient(ctx)
if err != nil {
	return nil, err
}
```

The result is an object with clients initialised for each service:
* `client.AuthorizeAPIClient`
* `client.CredentialsAPIClient`
* `client.ManagementAPIClient`
* `client.MFAAPIClient`
* `client.RiskAPIClient`
* `client.VerifyAPIClient`

In the above, if an `AccessToken` is provided, this will be verified and used.  If the `AccessToken` is not provided, the SDK will retrieve an access token from the provided `ClientID`, `ClientSecret`, `EnvironmentID` and `RegionCode` parameters.

The client SDK defaults to production hostnames, and the `RegionCode` is used to add the relevant suffix to the hostname.  For example, `EU` as a `RegionCode` value with suffix the service hostname with `.eu`.  Hostnames can be overridden with the optional `APIHostnameOverride`, and `AuthHostnameOverride` parameters.

An API call can be made against the API objects, as in the following example to get all environments in a tenant:

```go
...

resp, r, err := client.ManagementAPIClient.EnvironmentsApi.ReadAllEnvironments(ctx).Execute()
if err != nil {
	return nil, err
}
...
```
