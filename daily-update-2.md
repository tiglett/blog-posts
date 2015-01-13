# Daily update [28/01/2014]
Today was a busy day. Most of the previous UI issues have been solved, and a lot of progress has been made on the app.

For most of the day I was working on getting the camera functionality added. It’s now possible to add a picture to a Point of Interest. This was harder than expected, as it gives you a URI in a “picture:/path” form, where the path section is not a valid filesystem location. It requires the use of several classes and functions just to find the location on the filesystem for the picture, but at least it’s solved now.

The uploading is also nearly finished. The JSON is correctly formed, the app has the right permissions, and the user is given a “please wait” style dialogue until uploading is done. Once the upload either fails or finishes, this is closed and they are informed of the outcome. Tomorrow will probably be a day for final touches, bug fixes, and finishing off the uploading (it currently does not actually wait for the http response, and assumes that the sending was a success as long as the page exists).

 
Hours spent today:
  - 9am-5pm work in B23: 7 hours
  - Additional time after 5: 1 hour
  - Total so far: 37 hours
