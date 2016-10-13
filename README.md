#Guardian
An app that helps you get home safely.

This was our final project at DevBootcamp. Using a combo of app + hardware, we used a Parrot AR.Drone 2.0 to monitor User's progress for short (up to 10 minute) walks. Future iterations would include the feature of a drone auto-following user. 

##Images
![images](/animated.gif "images")

##Features

####Push the Walk Me Home button
* Drone lifts off
* Drone begins video recording
* Text message sends to friend with link to video stream

####Enter location
* Geolocation map is added to video stream page so that friend knows exactly where user is

####Live connection communication
* Friend clicks button across top of screen to indicate they're watching
* User's phone is updated to say that their friend is watching  

  **Challenge:** How to have one server responding to both User and Friend's clients.  

  **Solution:** Use setInterval function with a heartbeat to monitor change in event state.

####Push the Safe button upon arrival
* Lands the drone
* Ends video stream
* Triggers change in friends view

##Team
* Jason Lorentzen @codejlo
* Shawn Tuttle @shawnte
* Armon Arcuri @armoney
* Eric Booker @ericbooker12

##My Role
Initial program vision and mockups. Node API for connecting the drone to the internet, accept requests from rails app, and transmit live video stream. Created 'heartbeat' style pings from user apps to the server to allow notifications between users. Wrote CSS styling. Troubleshooting for API and database queries.
