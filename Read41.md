# Intent Filter

to Added an `Intent Filter` 

>The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

## Action

>A string naming the action to perform. Usually one of the platform-defined values such as ACTION_SEND or ACTION_VIEW.

## Data

>A description of the data associated with the intent.

>Specify this in your intent filter with the `<data>` element. Using one or more attributes in this element, you can specify just the MIME type, just a URI prefix, just a URI scheme, or a combination of these and others that indicate the data type accepted.

## Category

>Provides an additional way to characterize the activity handling the intent, usually related to the user gesture or location from which it's started. There are several different categories supported by the system, but most are rarely used. However, all implicit intents are defined with CATEGORY_DEFAULT by default.

## Handle the Intent in Your Activity

>In order to decide what action to take in your activity, you can read the Intent that was used to start it.

>**As your activity starts, call getIntent() to retrieve the Intent that started the activity. You can do so at any time during the lifecycle of the activity, but you should generally do so during early callbacks such as onCreate() or onStart().**

