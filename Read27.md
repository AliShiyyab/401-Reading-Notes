# Intents, Activities, and SharedPreferences

## Intent

>**Definition :** Is a messaging object you can use to request an action from another app component. An intent is an abstract description of an operation to be performed. It can be used with startActivity to launch an android.app.

>**Example Code :**

    Intent in=new Intent(MainActivity.this,NextActivity.class);
    startActivity(in);

>------------------------------------

## Activity

>**Definition :** Is the items did, like if the button when i clicked send me the other page ... the activities is the sending to other page.

>**Example Code :** 

    <activity
        android:name="com.shirish.Intent.NextActivity"
        android:label="@string/title_activity_next"
        android:parentActivityName="com.shirish.Intent.MainActivity" >
    <meta-data
        android:name="android.support.PARENT_ACTIVITY"
        android:value="com.shirish.Intent.MainActivity" />


>**Example of Activities :**

* *Button*
* *List Box*
* *Radio Button*
