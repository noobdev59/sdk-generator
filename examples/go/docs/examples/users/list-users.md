# Users Examples

## ListUsers

```go
    package appwrite-listusers

    import (
        "fmt"
        "os"
        "github.com/appwrite/go-sdk"
    )

    func main() {
        // Create a Client
        var clt := appwrite.Client{}

        // Set Client required headers
        clt.SetProject("")

        // Create a new Users service passing Client
        var srv := appwrite.Users{
            client: &clt
        }

        // Call ListUsers method and handle results
        var res, err := srv.ListUsers()
        if err != nil {
            panic(err)
        }

        fmt.Println(res)
    }
```