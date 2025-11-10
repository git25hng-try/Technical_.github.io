# Technical features and technologies of Smart vision care

## Technical blueprint 

[figure 1] (https://www.canva.com/design/DAG4MghuWF8/TDy-sWumlRZKEmDoF4QhJg/edit?utm_content=DAG4MghuWF8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

### Key features and Technologies 
***Features*** (MOSCOW)

MUST HAVE 
* Must have a spectrophotometer eye sensor
* Must have a book mode 
* Must have an accurate victual eye test detector
* Must have an accurate Cambridge color eye test detector
* Must have multiple users' average vision calculator for screen display
  from eye test results of intended users.

SHOULD HAVE 
* A GPS tracker
* A self-selected user font option
* A self-selected user brightness display
* A user option range for book mode
* A Device Detector
* Medical user eye test input

COULD HAVE
* A location color temperature
* A time of the day display color.

***Modules***
- Eye test module
- Eye sensor module
- Book mode selection module
- Screen display resolution modules

***Technical Communication***

|Frontend|Channel|Backend|Channel|Database request|Database store|
|-------|--------|-------|-------|--------|--------|
|Request for username|Server|Get CHARACTERS|Query|Device Keyboard and language settings|
|Request for user_id|API|Get DEVICE_ID|Query|Developers 'About Device'|Unique user_id|
|Request victual eye test|API|Get FONT SIZES-different alphanumeric, alphabets, and numbers for users to identify|Query|Device keyboard and language settings|Users' accurate font size|
|Request Cambridge color eye test|API|Get COLORS and COLOR NAMES|Query|Color Palettes and Schemes, Color Pickers and Eyedroppers|Users' accurate screen display resolution|
|Request Spectrophotometer eye test|API|Get EYE SENSOR-to monitor rays and eye coordination|Query|User permission.EYE_TRACKING|EYE_RAY sensitivity|
|Select book mode|Server|Get BOOK COLORS - without blue rays||
|Request screen display resolution|Server|Get EYE_TEST_RESULTS|App EYE_TEST Database store|User_ID and screen display|

***Technical Feasibility***
Smart vision care is technically feasible, but difficulties of integrating EYE_TEST parameters may exist.
