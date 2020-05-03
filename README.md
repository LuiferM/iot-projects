# Step Counter and Prediction with Weather Information
Summary: Based on Microbit, Rasperry Pi and Android phone, our team developed a step counter and made prediction of steps with weather information. <br>
Microbit: 
1. Collected step counts as # of shakes. 
2. Integrated with local storage and reset function. 
3. Able to send collected data to Rasperry Pi via bluetooth or radio broadcasts.

Rasperry Pi: Worked as backend. 
1. Received data from Microbit and stored in local filesystem.
2. Received weather information from Android phone.
3. Dynamically trained a linear regressor with gathered data.
4. Predict future steps according to historical steps and weather.
5. Send real steps and predicted steps to Android Phone.

Android Phone:
1. Gathered weather information via RESTful APIs.
2. Sent weather information to Rasperry Pi.
3. Displayed steps on UI.
