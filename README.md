# github.com/speakeasy-sdks/clearbit-dev-go

<!-- Start SDK Installation -->
## SDK Installation

```bash
go get github.com/speakeasy-sdks/clearbit-dev-go
```
<!-- End SDK Installation -->

## SDK Example Usage
<!-- Start SDK Example Usage -->
```go
package main

import (
    "context"
    "log"
    "github.com/speakeasy-sdks/clearbit-dev-go"
    "github.com/speakeasy-sdks/clearbit-dev-go/pkg/models/shared"
    "github.com/speakeasy-sdks/clearbit-dev-go/pkg/models/operations"
)

func main() {
    s := clearbit.New()

    ctx := context.Background()    
    req := operations.FindRequest{
        Company: "Medhurst - Rau",
        CompanyDomain: "quibusdam",
        Email: "Ryan.Little62@yahoo.com",
        Facebook: "deserunt",
        FamilyName: "suscipit",
        GivenName: "iure",
        IPAddress: "magnam",
        Linkedin: "debitis",
        Location: "ipsa",
        Twitter: "delectus",
        WebhookURL: "tempora",
    }

    res, err := s.Find(ctx, req)
    if err != nil {
        log.Fatal(err)
    }

    if res.Person != nil {
        // handle response
    }
}
```
<!-- End SDK Example Usage -->

<!-- Start SDK Available Operations -->
## Available Resources and Operations

### Clearbit SDK

* `Find` - Look up a person by their email address
<!-- End SDK Available Operations -->

### Maturity

This SDK is in beta and therefore, we recommend pinning usage to a specific package version.
This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

### Contributions

While we value open-source contributions to this SDK, this library is generated and maintained programmatically.
Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !

### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
