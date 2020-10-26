# Web Logs

## View Logs

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Logs" link on the Left Nav

_And_ the Developer selects the "App" from the combo

_Then_ List of all the Logs associated with the "App" are shown

_And_ the columns of the list should have Time, Severity, Origin Service, Message

_And_ Default order is Time.

## Filter Logs

_Given_ Developer is logged in to Developer Dashboard

_When_ Developer clicks the "Logs" link on the Left Nav

_And_ the Developer selects the "App" from the combo

_And_ the Developer selects the Filter for Severity as "CRITICAL"

_Then_ the Log list is shown with all the "CRITICAL" logs.
