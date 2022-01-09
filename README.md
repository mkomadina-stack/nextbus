# nextbus
iOS app that checks with SamTrans API for next available bus on routes

Completed project for iOS class. Below was original proposal


- "NextBus" iPhone app
- Purpose:  An easier way to check and remind students when the next buses are leaving campus
- Use the SamTrans Beta Bus API (XML URL)  (http://511.org/developer-resources_transit-api.asp) to get bus departure times from Cañada.  I've already gotten a developer token id and can see the XML in a browser.  

The idea is to create a simpler interface than having to check bus routes and schedules, with the possibility of a reminder to catch the bus.  

Primary use case is I'm a student on campus and I want to grab some food/meet friends/study at library but still catch my bus.  I just want to see when the next few buses are coming. 

Minimum viable product (project goal):  Real-time fetch and displays of departing bus times at Cañada campus stop displayed in an iOS app.  Enhancements could include setting a reminder alert and possibly switching bus stops along the route.

The project would demonstrate:
- iOS UI elements including likely table view,  ...
- Multiple classes including Bus, Route, ..
- Real-time data fetch using NSURLConnection
- Parsing the XML likely using NSXMLParser
- Displaying and persisting times (in case of connection loss)

Anticipated challenges:
- Determining the frequency of making the API call (periodic vs. on demand?)
- Handling disconnected states (what to do/show if no longer getting updates)  
- Any changes SamTrans makes to the API
- Setting and handling reminder alerts (if I get to enhancement)
- API shows 90 minute window.  How to best inform the user that it's not the full schedule.  This is a limitation of the API.
