# Project Plan

Pod Members: Daniel O, Michael S, Joy R

## Problem Statement and Description

This website allows users to enhance their resume by giving automated suggestions and feedback to tailor to their professional goals. 
Mission: Use automation to guide/ improve  the resume development process. 

## User Roles and Personas

User Roles
Two user roles are: Authenticated users: allowed to import and export resume Non-authenticated: can access landing/ get started page

User Personas
Freshman in College (Student) Stay-at-home Mom transitioing back to work High School Teacher showing students how to craft a resume Financial advisor looking to improve resume by adding specific words and phrases specific to his field

## User Stories

As an authenticated user, I want to see an "export complete pop-up", so that I know that the document was exported to my machine successfully.
As an authenticated user, I want to log in, so that I can use the product.
As an authenticated user, I want to open "the suggestion tab", so that I can view all of the generated suggestions.
As an authenticated user, I want to login and open my "personal account" page, so that I save and edit personal data.
As an authenticated user, I want to remain logged in and access previously updated resumes, so that all my resumes/ versions are in one place.
As a non-authenticated user, I want to see steps, so that I can better understand how the product works before creating an account.
As an authenticated user, I want to export my resume, so that I can send it to future employeers.
As an authenticated user, I want to edit my resume within the file, so that I don't have to copy, paste, and reformat my previous resume.
As a non-authenticated user, I want click a "learn more" button, so that I can see examples of how the product is being used.
As an authenticated user, I want to upload / drag and drop my resume in a designated box, so that it is clear that I am putting my document in the correct desired field.
As an authenticated user, I want to see my uploaded document in a new page, so that I know that the document was uploaded successfully and ready to edit.

## Pages/Screens

List all the pages and screens in the app. Include wireframes for at least 3 of them.
https://www.figma.com/file/OY1zfc1y2imnKPiEDKvzcO/Website-Wireframing-Template-%7C--The-Conference-Room-(Community)?type=whiteboard&node-id=0-1&t=Fm5UAhYZnByUg4qN-0 

## Data Model

Describe your app's data model using diagrams or tables

  |Users Table|  CATEGORIES                                        |            
  |-----------------------------------------------------------------                 
  |id         |  SERIAL PRIMARY KEY                                |
  |username   |  TEXT                                              |
  |password   |  TEXT                                              |
  |first_name |  TEXT                                              |
  |last_name  |  TEXT                                              |
  |email TEXT |  NOT NULL UNIQUE CHECK (position('@' IN email) > 1)|
  |created_at |  TIMESTAMP                                         |
  |updated_at |  TIMESTAMP                                         |


  |Resume Table:   |  CATEGORIES                     |               
  |---------------------------------------------------
  |id              | SERIAL PRIMARY KEY              |
  |url             | TEXT                            |
  |action_verbs    | JSON                            |
  |user_id INTEGER | FOREIGN KEY REFERENCES users(id)| 

## Endpoints

List the API endpoints you will need to implement.

Front end:
Log in 
/login (Post route) 
Registration endpoints
-  /Registration endpoints (post Route)
/upload
/database/addto (post Route)
/edit 
/synonyms  (get Route)
/actionsVerbs (get Route)
/adjectives (get Route)
/export
/database/getUrl (get route)
/AutomateRa  (landing Page)


***Don't forget to set up your Issues, Milestones, and Project Board!***
