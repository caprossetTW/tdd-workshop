## How to run 

Install the dependencies with:
```
npm install
```

Run tests with:
```
npm test
```


## Katas

### Kata 1 - Password input field validation

Create a function that can be used as a validator for the password field of a user registration form. The validation function takes a string as an input and returns a validation result. The validation result should contain a boolean indicating if the password is valid or not, and also a field with the possible validation errors.

#### Requirements
1. The password must be at least 8 characters long. If it is not met, then the following error message should be returned: “Password must be at least 8 characters”

2. The password must contain at least 2 numbers. If it is not met, then the following error message should be returned: “The password must contain at least 2 numbers”

3. The validation function should handle multiple validation errors.

For example, “somepassword” should an error message: “Password must be at least 8 characters\nThe password must contain at least 2 numbers”
4. The password must contain at least one capital letter. If it is not met, then the following error message should be returned: “password must contain at least one capital letter”

5. The password must contain at least one special character. If it is not met, then the following error message should be returned: “password must contain at least one special character”

&nbsp;   


### Kata 2 - Search functionality

Implement a city search functionality. The function takes a string (search text) as input and returns the found cities which corresponds to the search text.

#### Prerequisites
Create a collection of strings that will act as a database for the city names.

City names: Paris, Budapest, Skopje, Rotterdam, Valencia, Vancouver, Amsterdam, Vienna, Sydney, New York City, London, Bangkok, Hong Kong, Dubai, Rome, Istanbul

#### Requirements
1. If the search text is fewer than 2 characters, then should return no results. (It is an optimization feature of the search functionality.)

2. If the search text is equal to or more than 2 characters, then it should return all the city names starting with the exact search text.

For example for search text “Va”, the function should return Valencia and Vancouver
3. The search functionality should be case insensitive

4. The search functionality should work also when the search text is just a part of a city name

For example “ape” should return “Budapest” city
5. If the search text is a “*” (asterisk), then it should return all the city names.