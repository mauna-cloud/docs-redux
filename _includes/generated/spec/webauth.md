# Authentication Web Flow

## User logs in with valid credentials through github

_Given_ User is on Mauna home page

_When_ User clicks sign-in using github

_And_ User enters username and password for his github account registered with mauna

_Then_ User should be able to view his dashboard.

## Developer opens the Dashboard with expired token.

_Given_ Developer already has a token

_When_ the token is already expired

_And_ the expired token is sent to the Mauna Token Service

_And_ the token is checked by the MTS with the expiration date

_And_ Web page to sign-in using github is opened

_And_ User enters username and password for his github account registered with mauna

_Then_ User should be able to view his dashboard

_And_ the token is saved for future use.
