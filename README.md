# [FreeCodeCamp Timestamp Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/timestamp-microservice)
This is a Node.js application which is part of the FCC Back End Certification. It takes a date string and gives back a JSON with Unix value and UTC value for the given date.

# User stories:
> 1. A request to `/api/:date?` with a valid date should return a JSON object with a `unix` key that is a Unix timestamp of the input date in milliseconds (as type Number)
> 2. A request to `/api/:date?` with a valid date should return a JSON object with a `utc` key that is a string of the input date in the format: `Thu, 01 Jan 1970 00:00:00 GMT`
> 3. If the input date string is invalid, the api returns an object having the structure `{ error : "Invalid Date" }`
> 4. An empty date parameter should return the current time in a JSON object with a `unix` and `utc` keys

Example usage:
```
1. [project url]/api/2021-12-03
2. [project url]/api/1639008000000
3. [project url]/api/
4. [project url]/api/hello
```
Example output:
```
1. {"unix":1638489600000,"utc":"Fri, 03 Dec 2021 00:00:00 GMT"}
2. {"unix":1639008000000,"utc":"Thu, 09 Dec 2021 00:00:00 GMT"}
3. {"unix":1647598428838,"utc":"Fri, 18 Mar 2022 10:13:48 GMT"}
4. {"error":"Invalid Date"}
```