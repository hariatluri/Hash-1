# Testcases for /hash/1

## Scenario 1 Verify Encoded Password
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal "/hash"
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/1"
THEN system returns encoded password"

## Scenario 2 Verify using wrong encoded password in the endpoint and run in the command prompt ex:"6754676576"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN system returns encoded password"

## Defect Hash Not Found

## Scenario 3 Verify using negative wrong encoded password in the endpoint and run in the command prompt ex:"-76437676576"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/-76437676576"
THEN system returns encoded password"

## Defect Hash Not Found

## Scenario 4 Verify using Text encoded password in the endpoint and run in the command prompt ex:"JHGDHGJHDGJHG"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/JHGDHGJHDGJHG"
THEN system returns encoded password"

##  Defect Invalid syntax

## Scenario 5 Verify using special charecter encoded password in the endpoint and run in the command prompt ex:"^%$&^%&^^*&&*"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/^%$&^%&^^*&&*"
THEN system returns encoded password"

## Defect Invalid syntax

## Scenario 6 Verify using special charecter with "" inside the encoded password in the endpoint and run in the command prompt ex :"^% "  " &^*&"
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/^% "  " &^*&"
THEN system returns encoded password"

## Defect Invalid syntax command never exit's

## Scenario 7 Verify using empty space encoded password in the endpoint and run in the command prompt ex : 
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/"
THEN system returns encoded password"

## Defect Invalid syntax


## Scenario 8 Verify not running POST /hash endpoint  and run GET end point /hash/1
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN system returns encoded password"

## Defect Hash Not Found

## Scenario 9 Validate Get the base64 encoded password from /hash endpoint using Online tools
"GIVEN when the application is launched
WHEN port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
WHEN system returns encoded password"
THEN Verify encoded Password using Online tools

## Defect Encrpted password did not match free Online password encrption

## Scenario 10 Verify using wrong port
"GIVEN when the application is launched
WHEN Worng port is set
WHEN  User Enter the POST endpopint with password in the Terminal ""/hash""
WHEN User wait's for 5 seconds
WHEN system computes and returns Encripted Password
WHEN  User Enter the GET endpopint with password in the Terminal "/hash/76576"
THEN  Verify connection refused
