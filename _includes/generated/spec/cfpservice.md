# Context Frame Parser Service

## Context Frame Parser

_Given_ I have a valid token for mauna services

_When_ I call the  cfp.mauna.cloud with the token using the graphql query

_And_ Pass Context Object with userId and Content as String

_Then_ The cfp service will return Context Result with userId and the parsed string into tokens.
