# Testcases for /hash/1

## Scenario 1 Verify Encoded Password
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal "/hash"
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/1"
THEN system returns encoded password"

## Scenario 2 Verify using wrong encoded password in the endpoint and run in the command prompt ex:"76576"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN system returns encoded password"

## Scenario 3 Verify not running POST /hash endpoint  and run GET end point /hash/1
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN system returns encoded password"

## Scenario 4 Validate Get the base64 encoded password from /hash endpoint using Online tools
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
WHEN system returns encoded password"
THEN Verify encoded Password using Online tools

## Scenario 5 Verify using wrong port
"GIVEN when the application is launched
WHEN Worng port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN system returns encoded password"

