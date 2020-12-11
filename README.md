# itunes-api-cors

This repo contains a website that aims to reproduce an issue when performing CORS request against https://itunes.apple.com/search.

## Issue Description

When performing consecutive CORS requests against the iTunes Store API at
`https://itunes.apple.com/search` ([docs go
here](https://affiliate.itunes.apple.com/resources/documentation/itunes-store-web-service-search-api/))
from different origins in browsers on the same machine, the browser running the
second request will receive a response with the origin of the first request in
the `access-control-allow-origin` header.

[Open the website to reproduce the issue](https://teggno.github.io/itunes-api-cors/)
