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