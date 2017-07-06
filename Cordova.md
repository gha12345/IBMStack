

* [Integrating IBM MobileFirst Platform Foundation SDK in Cordova applications](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/hello-world/integrating-mfpf-sdk-in-cordova-applications/)


* [Integrating IBM MobileFirst Platform Foundation SDK in Cordova applications- Sampple](https://github.com/MobileFirst-Platform-Developer-Center/Cordova/tree/release71)

```bat
NAME
     mobilefirst cordova
SYNOPSIS
     mfp cordova <command> [options]
DESCRIPTION
     IBM MobileFirst Platform Command Line Interface (CLI) for Cordova specific
     actions.
     Specific help for each command is available. For example:
     mfp help cordova create
GLOBAL COMMANDS
     config .............................. View or alter configuration settings
PROJECT COMMANDS
     cordova create .............................. Creates a new Cordova project
     cordova emulate .................................. Emulates Cordova project
     cordova platform ................................ Manages project platforms
     cordova plugin .................................... Manages project plugins
     cordova prepare ............................... Prepares a Cordova project
     cordova preview ......................... Previews existing Cordova project
     cordova run .......................................... Runs Cordova project
COMMAND-LINE FLAGS/OPTIONS
     -v, --version ...............Prints out the version number of this utility
     -d, --debug ........................Debug mode produces a debug log output
     -dd, --ddebug ................... Debug mode produces a verbose log output
EXAMPLE USAGE
     $ mfp cordova create myapp --platform android
     $ cd myapp
     $ mfp cordova preview
     $ mfp cordova emulate --platform android

```


```bat

Warning: using node version v0.12.2 which has been deprecated. Please upgrade to the latest node version available (v6.x is recommended).
Synopsis

cordova command [options]

Global Commands
    create ........ Create a project
    help .......... Get help for a command
    telemetry ..... Turn telemetry collection on or off
    config ........ Set, get, delete, edit, and list global cordova options

Project Commands
    info .......... Generate project information
    requirements .. Checks and print out all the requirements for platforms specified
    platform ...... Manage project platforms
    plugin ........ Manage project plugins
    prepare ....... Copy files into platform(s) for building
    compile ....... Build platform(s)
    clean ......... Cleanup project from build artifacts
    run ........... Run project (including prepare && compile)
    serve ......... Run project with a local webserver (including prepare)

Learn more about command options using 'cordova help <command>'

Aliases
    build -> cordova prepare && cordova compile
    emulate -> cordova run --emulator

Options
    -v, --version ........... prints out this utility's version
    -d, --verbose ........... debug mode produces verbose log output for all activity,
    --no-update-notifier .... disables check for CLI updates
    --nohooks ............... suppress executing hooks (taking RegExp hook patterns as parameters)

Examples
    cordova create myApp org.apache.cordova.myApp myApp
    cordova plugin add cordova-plugin-camera
    cordova platform add android
    cordova plugin add cordova-plugin-camera --nosave
    cordova platform add android --nosave
    cordova requirements android    
    cordova build android --verbose
    cordova run android
    cordova build android --release -- --keystore="..\android.keystore" --storePassword=android --alias=mykey
    cordova config ls
    cordova platform add ios --nofetch
    cordova plugin add cordova-plugin-camera --nofetch
```

#Cordova project structure

After the Cordova project is created, the following files and folders are generated. This project structure follows the standard Cordova project structure:


* application-descriptor.xml - Application metadata for MobileFirst
* config.xml - The Cordova configuration file with extended MobileFirst-related preferences
* hooks - The Cordova hooks folder
* mobilefirst - The folder that contains MobileFirst artifacts: .wlapp files that MobileFirst Server needs to recognize applications, as explained below
* platforms - The folder that contains Cordova platforms support
* plugins - The folder that contains Cordova plug-ins
* www - The folder that contains the application web resources


![1](https://mobilefirstplatform.ibmcloud.com/assets/backup/cordova-project-structure.png)
![1](https://mobilefirstplatform.ibmcloud.com/assets/backup/cordova-app-1024x560.png)


```js
var Messages = {
    // Add here your messages for the default language.
    // Generate a similar file with a language suffix containing the translated messages.
    // key1 : message1,
};
var wlInitOptions = {
    // Options to initialize with the WL.Client object.
    // For initialization options please refer to IBM MobileFirst Platform Foundation Knowledge Center.
};
// Called automatically after MFP framework initialization by WL.Client.init(wlInitOptions).
function wlCommonInit(){
	// Common initialization code goes here
    document.getElementById('app_version').innerText = WL.Client.getAppProperty("APP_VERSION");
    document.getElementById('menu').setAttribute('style', 'display:block;');
}
var app = {
    // Application Constructor
    initialize: function() {
        this.bindEvents();
    },
    // Bind any events that are required on startup. Common events are:
    // 'load', 'deviceready', 'offline', and 'online'.
    bindEvents: function() {
        document.addEventListener('deviceready', this.onDeviceReady, false);
    },
    // The scope of 'this' is the event. In order to call the 'receivedEvent'
    // function, 'app.receivedEvent(...);' must be explicitly called.
    onDeviceReady: function() {
        app.receivedEvent('deviceready');
    },
    // Update the DOM on a received event.
    receivedEvent: function(id) {
		var parentElement = document.getElementById(id);
        var listeningElement = parentElement.querySelector('.listening');
        var receivedElement = parentElement.querySelector('.received');
        listeningElement.setAttribute('style', 'display:none;');
        receivedElement.setAttribute('style', 'display:block;');
        console.log('Received Event: ' + id);
    },
    // Trigger the vibration
    vibrate: function(){
        WL.Logger.info("vibrating");
        navigator.vibrate(3000);
    },
    // Trigger the camera
    getPicture: function(){
        navigator.camera.getPicture(app.getPictureSuccess, app.getPictureFail, { quality: 50,
            destinationType: Camera.DestinationType.FILE_URI });
    },
    // Receive the result from the camera
    getPictureSuccess: function(imageURI){
        WL.Logger.info("getPicture success "+imageURI);
        document.getElementById("image").src=imageURI;
    },
    // Called when some error occur with the camera
    getPictureFail: function(){
        WL.Logger.error("getPicture failed");
    },
    // Execute a request to RSSAdapter/getStories
    getRSSFeed: function(){
        var resourceRequest = new WLResourceRequest(
                    "/adapters/RSSAdapter/getStories",
                    WLResourceRequest.GET);
        resourceRequest.send().then(app.getRSSFeedSuccess,app.getRSSFeedError);
    },
    // Receive the response from RSSAdapter
    getRSSFeedSuccess:function(response){
        WL.Logger.info("getRSSFeedsSuccess");
        //The response.responseJSON element contains the data received from the back-end
        alert("Total RSS Feed items received:"+response.responseJSON.rss.channel.item.length);
    },
    // Called when some error occurs during the request to RSSAdapter
    getRSSFeedError:function(response){
        WL.Logger.error("Response ERROR:"+JSON.stringify(response));
        alert("Response ERROR:"+JSON.stringify(response));
    }
};
app.initialize();
```
