# Developing for Android
As I mentioned in my last post, I got the opportunity of going to the Android workshop today on behalf of our group – and I’m definitely glad I did.

I learned a lot about the differences between developing desktop Java apps and Java for Android. They are two completely different ways of doing things with different considerations that need to be remembered when developing. Fortunately it seems that creating the GUI for Android apps is quite easy – it’s all defined in XML, and IDEs such as Eclipse or Android Studio there’s a built-in WYSIWYG UI editor too.

Another really useful feature are the Android Intents. They allow you to easily perform actions internal to your app or using external apps and can give and receive data. This means that, for example, you could start an action to take a picture with the camera and use the data it returns as the image captured. This can string several apps together to form what would appear to the user as seamless integration.

As far as pit-falls go it seems the biggest is probably that your app can be paused/resumed upon certain events. This causes issues when rotating between landscape and portrait as the UI is destroyed and rebuilt. This means any data stored in the UI elements (entered text etc.) is lost. To overcome this the onCreate() method of your app, which is called as it is launched, can take a Bundle object as an argument. As a Bundle is just a list of key-value pairs it means you can store whatever data you want in it. This means you can simply store any necessary data in a Bundle when your app is killed and have code in your onCreate() method to deal with it.


I’m sure there’s a lot more I could write about Java on Android, but these are (to me) some of the most interesting parts.

Hours spent this week:
  - Internal meeting: 1 hour
  - Android workshop: 3 hours
  - Total this week: 4 hours
  - Total so far: 4 hours
