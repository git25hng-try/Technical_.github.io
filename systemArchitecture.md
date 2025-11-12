h# Technical features and technologies of Smart vision care

## Technical blueprint 

[figure 1] (https://www.canva.com/design/DAG4MghuWF8/TDy-sWumlRZKEmDoF4QhJg/edit?utm_content=DAG4MghuWF8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

### Key features and Technologies 
***Features*** (MOSCOW)

MUST HAVE 
* Must have a spectrophotometer eye sensor - This monitors and controls automatically users' vision to adjust screen display to sensitivity to blue rays.
* Must have a book mode - A no blue ray mode.
* Must have an accurate victual eye test detector - This detects the accurate font for users across all applications.
* Must have an accurate Cambridge color eye test detector - Checks for accurate color display for users' vision and adjusts screen brightness.
* Must have multiple users' average vision calculator for screen display
  from eye test results of intended users.

SHOULD HAVE 
* A GPS tracker - Activate location tracking permission to adjust screen brightness as such.
* A self-selected user font option
* A self-selected user brightness display
* A user option range for book mode
* A Device Detector
* Medical user eye test input - Users can input medical eye test result for screen display to protect their vision.

COULD HAVE
* A location color temperature - Requests users' permission to set screen display according to location.
* A time of the day display color - Screen displays according to users'time of the day.

***Modules and User stories***
|***Modules***|***Description***|***User story***|
|-------------|-----------------|----------------|
|Eye test module|Conducts user victual eye test and cambridge color test with accuracy|As a user, I want an application that can accurately test the font size and screen display colour that is compatible with my vision. I would not need to manually select, because it can be inaccurate.|
|Eye sensor module|Monitors users' vision and eye coordination to adjust screen display| As a user, I would prefer an application that can monitor my eye coordination and automatically set the blue ray illuminance while using the smart screen. The sensor observes dizziness or fatigue and adjust screen display to reflect that or give me a prompt on my eye coordination and ask for permission to adjust screen display or shut down the screen.|
|Book mode selection module|Ensures users are able to select a no blue ray mode|As a user, I want to be able to select the book mode, so that my screen reflects no rays, but that similar to just reading a hard copy book or pictures on the screen. I want a screen display mode that would not make me averse to reading hard copy books|
|Screen display resolution modules|Ensures that screen display is according to users' eye test result to protect their vision|As a user, I want my screen resolution display to protect my vision completely, regardless of the length of time I spend on the screen. I would not eventually have blurry vision, eye strain or sleep disturbances|

***Technical Communication***

|Frontend|Channel|Backend|Channel|Database request|Database store|
|-------|--------|-------|-------|--------|--------|
|Request for username|Server|Get/CHARACTERS|Query|Device Keyboard and language settings|Stores username|
|Generate user_id|API|Get/DEVICE_ID|Query|Developers 'About Device'|Unique user_id|
|Request victual eye test|API|Get/FONT SIZES-different alphanumeric, alphabets, and numbers for users to identify|Query|Device keyboard and language settings|Users' accurate font size|
|Request Cambridge color eye test|API|Get/{COLORS}/{COLOR NAMES}|Query|Color Palettes and Schemes, Color Pickers and Eyedroppers|Users' accurate screen display resolution|
|Request Spectrophotometer eye test|API|Get/EYE SENSOR-to monitor rays and eye coordination|Query|User permission.EYE_TRACKING|EYE_RAY sensitivity|
|Select book mode|Server|Get/BOOK COLORS - without blue rays||
|Request screen display resolution|Server|Get EYE_TEST_RESULTS|Query|App EYE_TEST Database store|User_ID and screen display resolution|

***Technical Feasibility***
Smart vision care is technically feasible, but difficulties of integrating EYE_TEST parameters may exist.
|***Module***|***Technical difficulty***|
|------------|---------------------------|
|Eye test|Medium|
|Eye sensor|High|
|Book mode selection|Easy|
|Screen display resolution|High|
