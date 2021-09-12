# Cognito

## Configure Auth Category

To start provisioning auth resources in the backend, go to your project directory and **execute the command:**

>**`amplify add auth`**

## Install Amplify Libraries

>Add the following dependency to your app's build.gradle along with others you added above in Prerequisites and click "Sync Now" when prompted:

    dependencies {
        implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'
    }

## Initialize Amplify Auth

>Add the Auth plugin before calling Amplify.configure. Update the code you added in Prerequisites:

    // Add this line, to include the Auth plugin.
    Amplify.addPlugin(new AWSCognitoAuthPlugin());
    Amplify.configure(getApplicationContext());

