# SSML Service

## Convert Speech Markup using Voice CSS

_Given_ I have a valid token for mauna services

_When_ I call the  ssml.mauna.cloud with the token using the graphql query

_And_ Pass the SSML string and VoiceCSS as String

_Then_ The SSML service should return new SSML Text after applying VoiceCSS.
