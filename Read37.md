# S3 Amazon

>**Steps:**

* `amplify add storage`
* `Content (Images, audio, video, etc.)`
* `Yes`
* `Default configuration`
* `Username`
* `No, I am done.`
* `S3friendlyName`
* `storagebucketname`
* `Auth and guest users`
* `create/update, read, delete`
* `create/update, read, delete`
* `No`
* `amplify push`
* `Added a dependencies` 

    implementation 'com.amplifyframework:aws-storage-s3:1.24.0'
    
    implementation 'com.amplifyframework:aws-auth-cognito:1.24.0'

* `Click Sync Now.`
* `In The Try:`

    Amplify.addPlugin(new AWSCognitoAuthPlugin());
    
    Amplify.addPlugin(new AWSS3StoragePlugin());

* 
* 