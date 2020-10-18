#AMAAR - Requirements 4,5,8
#BUCHI - Requirements 2,6
#AARTI - Requirements 3,7
#LIA - Requirements 1,6
|                                                                                                                Specification | Test case ID |                                                                                                          Purpose |
|-----------------------------------------------------------------------------------------------------------------------------:|-------------:|-----------------------------------------------------------------------------------------------------------------:|
| The name of the ticket has to be alphanumeric-only,<br> and space allowed only if it is not the first or the last character. |       R4.1.1 | Check if the selling actions succeed when <br>the ticket names is alphanumeric-only<br>and contains legal spaces |
| The name of the ticket has to be alphanumeric-only,<br> and space allowed only if it is not the first or the last character. |       R4.1.2 |     Check if the selling actions fail when <br>the ticket names contains special characters<br>or illegal spaces |
|                                                                       The name of the ticket is no longer than 60 characters |       R4.2.1 |                                          Check if selling actions succeed when <br>ticket name is less than 60ch |
| The name of the ticket is no longer than 60 characters                                                                       | R4.2.2       | Check if selling actions fail when ticket name<br>is less than 60ch                                              |
| The quantity of the tickets has to be more than 0, and less than or equal to 100.                                            | R4.3.1       | Check if selling actions succeed when quantity is within the bounds                                              |
| The quantity of the tickets has to be more than 0, and less than or equal to 100.                                            | R4.3.2       | Check if selling actions fail when quantity is not within the bounds.                                            |
| Price has to be of range [10, 100]                                                                                           | R4.4.1       | Check if selling actions succeed when price is within range.                                                     |
| Price has to be of range [10, 100]                                                                                           | R4.4.2       | Check if selling actions fail when price is not within the range.                                                |
| Date must be given in the format YYYYMMDD (e.g. 20200901)                                                                    | R4.5.1       | Check if selling actions succeed when date is valid                                                              |
| Date must be given in the format YYYYMMDD (e.g. 20200901)                                                                    | R4.5.2       | Check if selling actions succeed when date is invalid                                                            |
| For any errors, redirect back to / and show an error message                                                                 | R4.6.1       | Check if website is redirected to user profile page with error message when selling action fails                 |
| The added new ticket information will be posted on the user profile page                                                     | R4.7.1       | Check if new ticket information is posted on profile page is selling action succeeds                             |
| For any other requests except the ones above, the system should return a 404 error                                           | R8           | Check if 404 error message is displayed when user requests something invalid                                     |
| The name of the ticket has to be alphanumeric-only,<br> and space allowed only if it is not the first or the last character. |       R5.1.1 | Check if the update actions succeed when <br>the ticket names is alphanumeric-only<br>and contains legal spaces |
| The name of the ticket has to be alphanumeric-only,<br> and space allowed only if it is not the first or the last character. |       R5.1.2 |     Check if the selling actions fail when <br>the ticket names contains special characters<br>or illegal spaces |
|                                                                       The name of the ticket is no longer than 60 characters |       R5.2.1 |                                          Check if selling actions succeed when <br>ticket name is less than 60ch |
| The name of the ticket is no longer than 60 characters                                                                       | R5.2.2       | Check if update actions fail when ticket name<br>is less than 60ch                                              |
| The quantity of the tickets has to be more than 0, and less than or equal to 100.                                            | R5.3.1       | Check if update actions succeed when quantity is within the bounds                                              |
| The quantity of the tickets has to be more than 0, and less than or equal to 100.                                            | R5.3.2       | Check if update actions fail when quantity is not within the bounds.                                            |
| Price has to be of range [10, 100]                                                                                           | R5.4.1       | Check if update actions succeed when price is within range.                                                     |
| Price has to be of range [10, 100]                                                                                           | R5.4.2       | Check if update actions fail when price is not within the range.                                                |
| Date must be given in the format YYYYMMDD (e.g. 20200901)                                                                    | R5.5.1       | Check if update actions succeed when date is valid                                                              |
| Date must be given in the format YYYYMMDD (e.g. 20200901)                                                                    | R5.5.2       | Check if update actions succeed when date is invalid                                                            |
| For any errors, redirect back to / and show an error message                                                                 | R5.6.1       | Check if update is redirected to user profile page with error message when selling action fails                 |
| The added new ticket information will be posted on the user profile page                                                     | R5.7.1       | Check if new ticket information is posted on profile page is update action succeeds                             |
| If the user has logged in, redirect back to the user profile page                                                                       | R2.1.1  | check if the user has logged in and if so, go to user profile page                                                                                                                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------|---------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| otherwise, show the user registration page                                                                                              | R2.2.1  | check if user is logged in, if not, have  user register                                                                                                                                                                                                                     |
| the registration page shows a registration form requesting:  email, user name, password, assword2                                       | R2.3.1  | check if registration page contains  necessary fields                                                                                                                                                                                                                       |
| the registration page shows a registration form requesting:  email, user name, password, assword2                                       | R2.3.2  | check if registration page does not contain necessary fields                                                                                                                                                                                                                |
| The registration form can be submitted as a POST  request to the current URL (/register)                                                | R2.4.1  | check if registration page is a post request that sends it to database from current URL                                                                                                                                                                                     |
| The registration form can be submitted as a POST  request to the current URL (/register)                                                | R2.4.2  | check if registration page is a post request that sends it to database from current URL                                                                                                                                                                                     |
| Email, password, password2 all have to satisfy the  same required as defined in R1                                                      | R2.5.1  | check if email, password and password2  are valid(password minimum length 6, at least one  upper case, at least one lower case,  and at least one special character)  (neither can be empty),(email must follow defined format)                                             |
| Email, password, password2 all have to satisfy the  same required as defined in R1                                                      | R2.5.2  | check if email, password and password2  are not valid, if they violate any of the following: (password minimum length 6, at least one  upper case, at least one lower case,  and at least one special character)  (neither can be empty),(email must follow defined format) |
| Password and password2 have to be exactly the same                                                                                      | R2.6.1  | check if password is the same as password2                                                                                                                                                                                                                                  |
| Password and password2 have to be exactly the same                                                                                      | R2.6.2  | check if password is not the same as password2                                                                                                                                                                                                                              |
| User name has to be non-empty, alphanumeric-only, and space  allowed only if it is not the first or the last character.                 | R2.7.1  | check if username is the non-empty, alphanumeric-only and space allowed only if it is not the first or  the last character                                                                                                                                                  |
| User name has to be non-empty, alphanumeric-only, and space  allowed only if it is not the first or the last character.                 | R2.7.2  | check if username is empty, has special character, and space  in first position or last                                                                                                                                                                                     |
| User name has to be longer than 2 characters  and less than 20 characters.                                                              | R2.8.1  | check if username is in between 2 and 20 characters long                                                                                                                                                                                                                    |
| User name has to be longer than 2 characters  and less than 20 characters.                                                              | R2.8.1  | check if username is not in between 2 and 20 characters long                                                                                                                                                                                                                |
| For any formatting errors, redirect back to /login and show message  '{} format is incorrect.'.format(the_corresponding_attribute)      | R2.9.1  | check if there are no formatting errors                                                                                                                                                                                                                                     |
| For any formatting errors, redirect back to /login and show message  '{} format is incorrect.'.format(the_corresponding_attribute)      | R2.9.2  | check if there are formatting errors                                                                                                                                                                                                                                        |
| If the email already exists, show message 'this email has been ALREADY used'                                                            | R2.10.1 | check if email does not already exist                                                                                                                                                                                                                                       |
| If the email already exists, show message 'this email has been ALREADY used'                                                            | R2.10.2 | check if email already exists                                                                                                                                                                                                                                               |
| If no error regarding the inputs following the rules above,  create a new user, set the balance to 5000, and go back to the /login page | R2.11.1 | check if any input errors                                                                                                                                                                                                                                                   |
| If no error regarding the inputs following the rules above,  create a new user, set the balance to 5000, and go back to the /login page | R2.11.2 | check if any input errors                                                                                                                                                                                                                                                   |