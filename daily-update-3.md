# Daily update [29/01/2014]
Today I spent mostly fixing bugs and making the app overall more polished. Most Activities no longer lose their data when the screen is rotated after overriding their onSaveInstanceState methods.

The only thing left to do with the UI is to disable the upload button and lock the screen orientation whilst the http requests are being sent. This is because if the screen is re-oriented then the AsyncTask is still running, and when it attempts to show the dialogs (which no longer exist/have associated activities) it crashes.

As well as this, i’m also considering killing the AsyncTask in the onSaveInstanceState. This will allow for the activity to be closed and re-opened, whilst not doing anything in the background and not informing the user.

Currently the only bug which seems difficult to fix is occuring in communication between the app and the server. Sometimes the app uploads correctly, and sometimes it reports it uploads and nothing is added to the database. After speaking with the web development team, it seems like it could be an issue with encoding and escaping the JSON with the base64 strings used for images. This is because the data always reaches the server as the app always receives a 200 OK from it.

Hours spent today:

 * 9am-5pm work in B23: 7 hours
 * Additional time after 5: 1 hour
 * Total so far: 45 hours
