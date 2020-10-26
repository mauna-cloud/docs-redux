# Authentication SDK

## Developer tries to use cli without any token or invalid token

_Given_ Developer does not have a valid token

_When_ Developer runs any mauna command on the shell

_Then_ cli prints a message to run mauna auth:login command

_And_ Prints the help with all the command options.

## Developer runs mauna auth:login command authenticated

_Given_ Developer is already logged in

_When_ when Developer runs auth:login command

_Then_ The mauna cli prints "Already Athenticated".

## Developer runs mauna auth:login command un-authenticated on GitHub

_Given_ Developer is NOT logged in

_When_ when Developer runs auth:login command

_And_ Developer is not already authenticated on the Web

_Then_ The mauna cli opens up the token fetching web page

_And_ waits for token process to finish

_And_ Saves the token to the local file.

## Developer runs mauna auth:login command un-authenticated on GitHub

_Given_ Developer is already logged in

_When_ when Developer runs auth:login command

_And_ Developer is already authenticated on the Web using the GitHub account

_Then_ The mauna cli call the Mauna token service

_And_ Mauna token service returns the token generated for the GitHub account

_And_ Saves the token to the local file.

## Developer wants to check authentication status after successful authentication

_Given_ Developer is already authenticated

_When_ when Developer runs auth:status command

_And_ the token is not saved in the local file

_Then_ The mauna cli call the Mauna token service

_And_ Mauna token service returns the token generated for the GitHub account

_And_ Saves the token to the local file.

## Developer wants to check authentication status

_Given_ Developer is NOT already authenticated

_When_ when Developer runs auth:status command

_And_ the token is not saved in the local file

_Then_ The mauna cli call the Mauna token service

_And_ Mauna token service returns "token not valid".

## Developer wants to check authentication status on expired token

_Given_ Developer is already authenticated

_When_ when Developer runs auth:status command

_And_ the token in the local file is already expired

_Then_ The mauna cli call the Mauna token service with the token

_And_ Mauna token service returns "token has already".

## Developer wants to authenticate on expired token

_Given_ Developer is already authenticated but with expired token

_When_ when Developer runs auth:login command

_And_ the token saved in the local file has expired

_Then_ The mauna cli call the Mauna token service

_And_ Mauna token service returns the token generated for the GitHub account

_And_ Saves the token to the local file.
