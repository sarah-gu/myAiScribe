

# myAIScribe

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
Mobile app to keep track of your coursework history, grades, and plan for upcoming semesters

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:** Lifestyle / Social / Utility
- **Mobile:** Easy to access notes-viewing on your phone, more accessible than a webpage that you need to navigate to
- **Story:** Creates a seamlined and all-in-one-place view of notes, with ML automatically highlighting the phrases and keywords. 
- **Market:** Any student can use this app. 
- **Habit:** Students use the app to keep track of their notes, and have a faster note-taking system altogether. Additionally, students can use the app to create goals for their note-taking and study habits. 
- **Scope:** V1 could be the basic scanning / storing notes setup without any ML function. V2 would expand to incorporate CoreML image to text translator (search function). V3 would add in ability to track graphs set goals. V4 stretch goal incorporate user field subject and highlight based on user input. 

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User can log in / create account
* User can take pictures of notes 
* User can view the stored notes and filter by subject or by recent date of addition
* Settings page for basic profile information display



**Optional Nice-to-have Stories**

* Goals page with pie charts showing the status of the goal 
* Reminders tab to set reminders about completing goals/ studying
* General graphs page showing trends of learning over the history of using the app 

### 2. Screen Archetypes

* Login Screen
   * user logs in
* Register Screen
   * user registers for an account
* Scanner Screen
   * user can take picture of notes
* Notes Display 
   * User can view the stored notes and filter by subject or by recent date of addition
* Settings Screen
   * Settings page for basic profile information display

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Scanner
* Note Display
* Settings

**Flow Navigation** (Screen to Screen)

* Login Page
   * Notes Display
* Notes Display
   * Scanner
   * Settings
* Settings
   * Goals
   * Reminders
   * Notes Display
   * Login Page
   * Scanner

## Wireframes

![figma wireframes](https://github.com/sarah-gu/myAIScribe/blob/main/figma.png)


### Models
- Notes model, has info about the subject and image to be uploaded. 
### Networking
- Send requests to the CoreML API 
- Parse Network uploads a new Note 

## Work Plan 
**Required MVP Stories**
* Week 1
  * Set up the general workflow of required User Stories mentioned above (LoginViewController, SettingsViewController, NotesViewController, ScannerViewController) [1-2 days]
  * Try out a simple CoreML feature of text recognition [1 day]
  * Integrate the CoreML feature into the app, doing a basic image to text translation system. At the same time, expand the Notes model to incorporate more fields, such as adding a subject tag when uploading a Note to the backend. [1-2 days] 
* Week 2
  * Use the text translated from CoreML to create different tabs for the Notes page, i.e filtering by Class, time created, subject. [1-3 days] 
  * Create new pages for the Goals & reminders tabs, adding more view controllers for different tabs in the Settings page. [1-2 days]
**Stretch Goals**
* Week 3 
  * Integrate a visualization API to the Goals page, adding animation + customization features. [1 day]
  * Add additional ML features of suggesting similar classes / notes based on uploaded notes and subjects. [1-2 days] 
  * Add a search bar for notes based on the text translation from CoreML. [1-2 days] 
* Week 4 & 5
  * Put final touches on app & prepare for demo







