```
dotnet add package Microsoft.AspNetCore.Authentication.Cookies --version 2.2.0
dotnet add package Microsoft.AspNetCore.Authentication.OpenIdConnect --version 3.1.10
```


## Snippets

`Starup.cs`
```
    ...
    app.UseCookiePolicy(); 
    app.UseAuthentication();
    ....
```

`appsettings.json`
```
....
"Auth0": {
    "Domain": "{Domain}",
    "ClientId": "{ClientId}",
    "ClientSecret": "ClientSecret"
},
...
```


## Credits
* [auth0/aspnet-core-3/01-login](https://auth0.com/docs/quickstart/webapp/aspnet-core-3/01-login)