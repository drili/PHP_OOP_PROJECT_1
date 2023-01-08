# PHP OOP Project #1

### Prerequisites
    - Apache Server
    - MySql Database
    - Composer
        - Dependencies:
            * https://github.com/vlucas/phpdotenv
    - .env setup

##### Composer install depenendies
```$ composer require vlucas/phpdotenv```

##### Variable composition @ .env
```
HOSTNAME=""
USERNAME=""
PASSWORD=""
DATABASE=""
```

##### Define "$root_directory" @ "../parts/header_pre.php"
```
$root_directory = $_SERVER['DOCUMENT_ROOT'] . "{{YOUR_PROJECT_DIRECTORY_NAME}}";
```

### Task list
- [x] Setup dynamic directories
- [x] Setup folder and file structure
- [x] Setup database connection
- [x] Add composer dependency for .env file
- [x] Add libraries: CSS Foundation ZURB, jQuery and reset CSS
- [x] Setup "User" class & "users" table in database
- [x] Setup "Form" component
- [x] Setup "SuccessStatus" (js component) component
- [x] Create a "Login" form and use PHP to login the user using "email" and "password" as parameters.
    - Make sure the user gets redirected to the dashboard view
- [x] Add authentication controller, if user is not logged in, they must be redirected back to the login page.
    - Also check if the user is activated
- [x] Start CSS styling (global- and component-based styling)
- [x] Add SQL database to repo
- [x] Setup basic navigation (sidebar for main links, topnav for misc)
- [x] Setup darkmode functionality
    - Use database instead of cookies
    - Database updates when darkmode enabled/disabled
- [x] Profile page
    - User can update their profile, insert profile image
    - Stylize the profile page
- [x] Stylize the not-activated.php page
- [ ] Create "create_task" view
    - Create database table (async)
    - User be able to create task functionality, corresponding to table
    - Latest createt tasks by user async-fetch
- [ ] Task modal view
    - ...
- [ ] Setup "user_roles" table in database
- [ ] Admin view
    - Admin can activate un-activated users (also de-activate)
    - Admin can delete and modify users