# Key Value Storage Service

## Set Key Value storage for App

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql mutaiton

_And_ call the updateApplication with App Id

_And_ pass the Key string

_And_ pass the Value as JSON

_Then_ The Key-Value service should store the value with Key against the Aplication Id.

## Set Key Value storage for Session

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql mutaiton

_And_ call the updateSession with Session Id

_And_ pass the Key string

_And_ pass the Value as JSON

_Then_ The Key-Value service should store the value with Key against the Session Id.

## Set Key Value storage for an end-user

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql mutaiton

_And_ call the updateUser with User Id

_And_ pass the Key string

_And_ pass the Value as JSON

_Then_ The Key-Value service should store the value with Key against the User Id.

## Get the Value for a Key for a given Applicaton Id

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql query

_And_ call the getApplication

_And_ pass the applicaton Id

_And_ pass the Key string

_Then_ the JSON value corresponding the Key for the Application Id is returned.

## Get the Value for a Key for a given Session Id

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql query

_And_ call the getSession

_And_ pass the Session Id

_And_ pass the Key string

_Then_ the JSON value corresponding the Key for the Session Id is returned.

## Get the Value for a Key for a given end user Id

_Given_ I have a valid token for mauna services

_When_ I call the kvs.mauna.cloud with the token using the graphql query

_And_ call the getEndUser

_And_ pass the User Id

_And_ pass the Key string

_Then_ the JSON value corresponding the Key for the User Id is returned.
