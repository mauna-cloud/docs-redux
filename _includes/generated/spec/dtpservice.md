# Dialog Turn Prediction Service

## Dialog Turn Prediction

_Given_ I have a valid token for mauna services

_When_ I call the  dtp.mauna.cloud with the token using the graphql query

_And_ Pass the history as string and possible altternatives

_Then_ The DTP service should return dialog alternatives with a rank.
