# Ocom vue_interview_test

This the Ocom Vue Test 

# Setup Backend Server

- Clone this repository
- Download the json-server from here <https://github.com/chanioxaris/json-server/releases/tag/v1.0.0>
- Place the executable in this directory and then run

```bash
./json-server start
```

This will fire up a Test Server you can use as your API Server.
This will have the following routes:

Library
- **GET /library** - Get all Libraries
- **GET /library/:id** - Get A Library by ID
- **POST /library** - Create a new Library - will create an new ID
- **PUT /library/:id** - Update the Library with the :id specified
- **PATCH /library/:id** - Update some fields in the Library by the :id
- **DELETE /library/:id** - Delete the Library

Project
- **GET /project** - Get all Projects
- **GET /project/:id** - Get A project by ID
- **POST /project** - Create a new project - will create an new ID
- **PUT /project/:id** - Update the project with the :id specified
- **PATCH /project/:id** - Update some fields in the project by the :id
- **DELETE /project/:id** - Delete the project

There are sample curl lines to TEST the api server and show how it works.

# Project

I need a Vue 2 App using vue-cli that has the following screens

## List Project Items

A table of all the Projects.

Columns should be

- Name - When they click the Name it will edit the Project
- Client Name
- Production URL
- Test URL
- Git URL

## Edit Project Item

When the User clicks the Project Name they can edit the Project

The form will have the following fields

- Name
- Client Name
- Description
- Git URL
- Test URL
- Production URL
- Table of Libraries - This table will have two columns
  - Library - Select from the Library list
  - Version - A Text Input to enter the Version text.
- Active Start Date
- Active End Date

The user can add multiple lines to the Table Of Libraries
They can select only the Active Library entries. The Library entries are active if the active_end_date is null OR the date (when parsed) is after the current date AND the active_start_date is BEFORE the current date.

## Create Project Item

From the list of Projects they can press a button to create a new Project Item

The form will have the following fields (the same above)

- Name
- Client Name
- Description
- Git URL
- Test URL
- Production URL
- Table of Libraries - This table will have two columns
  - Library - Select from the Library list
  - Version - A Text Input to enter the Version text.
- Active Start Date - Default to Todays date.
- Active End Date

The "rest server" will add a new ID for you which is a random number.

The user needs to be able to Create a New Project Item, and return the list of Projects with the new Project included in the results.

# Expectations
When completing this task we expect to see the following
- You use Bootstrap CSS
 - Use Vue2
 - Use VueX
 - No Authentication is required as the test server doesn't support it :)
  - We are to see how you would code this. We know it's not perfect and feature complete.

# Documentation Test
Please add a  file to the Project that has the following

- Installation/Running Instructions (don't include running the json-server as above) so we can run git clone and follow the instructions to get the vue server running.
- Tell us what you would do different if you had more time
- Tell us what features you would add if you had more time




Good Luck and Have Fun!!!