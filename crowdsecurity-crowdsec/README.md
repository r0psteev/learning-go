# Package structure

`cmd/crowdsec`: this dir contains main binary for crowdsec daemon
`cmd/crowdsec-cli`: contains the cli to interact with the daemon

I know that there's a web dashboard too, where's it ?

# OpenApi

- `crowdsec/pkg/models/add_alerts_request.go` : imports go-openapi
This suggests the use of openapi within the project to preserve shared json structure accross communicating
components i guess.

This file also seems to be generated automatically from `swagger`.
I have the feeling at this point that the openapi stuffs works kind of like protobufs for code generation.