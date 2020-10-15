iOS Cordova CORS testing

Some scenarios I tried

| What to do                                    | Expected Output   | Actual Output     | Notes                                    |
|-----------------------------------------------|-------------------|-------------------|------------------------------------------|
| CORS request with cookies and no allow origin | fail              | fail              |                                          |
| CORS request with cookies and allow origin   | work              | fail              | Used to work until iOS 14/ITP enablement |
| Proxy requests                                | work all the time | work all the time |                                          |
| Proxy requests and then unproxied requests with allow origin| work | fail | Used to work until iOS 14/ITP enablement |
| Load image tags with cookies set | work | fail | Used to work until iOS 14/ITP enablement |