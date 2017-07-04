# IBM-MobileFirstPlatform

## Start Here

* [mfp.help](https://mfp.help/)
* [IBM MobileFirst Platform Foundation 8.0](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/)


# Mobile First Platform - Product Features

* **Comprehensive Security** - Protect from mobile specific threats

  * **Advanced Mobile Authentication** - Easily add advanced mobile authentication to your apps, including step-up, multi-factor, SSO between apps & between back-ends and more.
  * **App Authenticity** - App fingerprinting to prevent access to your APIs from malicious apps.
  * **Certificate Pinning** - Thwart Man-in-the-Middle attacks.
  * **Remote Disable & Version Enforcement** - Protect users from unsafe apps by disabling versions & forcing users to upgrade.
  * **Device Whitelisting & Blacklisting** - Protect from device loss, theft, or misuse.

* **App Lifecycle Management** - To reduce time and costs of operations and incremental updates
  * **Direct Update** - Push over-the-air changes to front end web resources without app store review. 
  * **Live Update** - Change your app on the fly, roll new features out gradually, A/B test, and customize your app for different users.

* **Mobile Analytics** - To better understand your users
  * **Crash Analytics** - Make sure your app is stable, and that you can fix problems quickly.
  * **App & API Performance Analytics** - Stay ahead of problems, and keep your app responsive.
  * **App Usage Metrics & Custom Business Metrics** - Understand your users and how they use your app.

* **Backend Logic Engine** - To add server side logic to your app
  * **Adapters** - Quickly develop & run server side code to communicate with your backend systems securely. Add your business logic, and make it dynamically configurable so you can change app behavior without recompile.
  * **Dynamic Set-up of App Security & Back-End Configuration** - Make changes in real-time to the app security configuration (eg. authentication method, max number of login attempts allowed) or backend configuration (eg. Database URL), with zero downtime or recompile.

* **Push & Offline Sync** - Essential backend services that every app needs
  * **Push and SMS Notifications** - Deliver messages to multiple platforms with a single API & send targeted messages from a web console.
  * **JSONStore** - Encrypted on device storage & automated data sync for better app performance & offline access.



## Tools

MobileFirst Development Kit bundles together the following components: 
* MobileFirst Server 
  * MobileFirst and the MobileFirst Server administration service
  * MobileFirst runtime
  * MobileFirst Server push service
  * MobileFirst Analytics and the MobileFirst Analytics Console
* MobileFirst Operations Console
* MobileFirst Command-line Interface (CLI)
* MobileFirst client SDKs 
* MobileFirst adapter tooling
* MobileFirst Plaform Fountation
* MobileFirst Studio
* MobileFirst Mobile Test Workbench

MobileFirst Server

Production Server
* IBM Installation Manager
* WebSphere Liberty profile v8.5.5.8
* MobileFirst Server for Production


## [Product Main Capabilities](http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/product-overview/capabilities/)
* Development
* Back-end connections
* Push notifications
* Offline mode
* Update
* Security
* Analytics
* Monitoring
* Application publishing


Matrix of features & platforms
http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/product-overview/features-matrix/



# [Developing Applications](http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/application-development/)
* Adding the MobileFirst SDK
* Using the MobileFirst CLI
* MobileFirst Eclipse plug-in
* Cordova application development
* Resource Requests
* JSONStore
* Client-side log collection
* Direct Update
* Multilingual translation
* Debugging applications
* Live Update
* Simple Data Sharing
* watchOS 2, watchOS 3

# [Developing Adapters](http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/adapters/)
* Creating Adapters
* JavaScript Adapters
* Java Adapters
* Developing Adapters in Eclipse
* Testing and Debugging Adapters
* Server-side log collection
* Adapter Mashup
* Integrating with Cloudant

# Authentication and Security
* Creating a security check
* Credentials Validation
* User Authentication
* Step Up Authentication
* ExternalizableSecurityCheck
* Enrollment
* LTPA Security Check
* Application Authenticity
* Confidential Clients
* Device SSO
* Protecting External Resources
* Certificate Pinning
* Configuring the Server Keystore

# Notifications
* Sending Notifications
* Handling SMS Notifications
* Handling Push Notifications
* Setting Up Analytics Support
* Push Service REST APIs

Analytics
* Analytics API
* Analytics REST API
* Elasticsearch
* Analytics Console
* Workflows


# Administering Applications
* Deploying apps to environments
* Administrating using the console
* Administrating using Ant
* Administrating using terminal
* Federal standards support
* License tracking


# Application Center
* Preparations
* Push notifications
* The Application Center console
* Uploading or deleting an app
* The mobile client
* Setting up logging and tracing



Foundation
Developers
Admins


## [Product Components](http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/product-overview/components/)
* MobileFirst CLI
* MobileFirst Server
* Client-side runtime components
* MobileFirst Operations Console
* MobileFirst Application Center
* MobileFirst System Pattern

![1](http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/product-overview/components/architecture.jpg)



IBM MobileFirst Platform Foundation-http://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/8.0/api/client-side-api/

MobileFirst Server
IBM MobileFirst Platform Studio is an Eclipse plug-in
MobileFirst CLI
MobileFirst Platform Operations Console


Server-side development
	JavaScript adapters
	Java Adapters
JSONStore

Notifications
Analytics
Foundation on Bluemix
Application Center



## API Connect

* [Getting Started](https://developer.ibm.com/apiconnect/getting-started/)
* [IBM API Connect: new approach for API management](https://www.youtube.com/watch?v=lmxyiNMER5Y)
* [Introducing IBM API Connect](https://strongloop.com/strongblog/introducing-ibm-api-connect/)

## MFP

## Bluemix

## Watson



https://www-304.ibm.com/services/learning/ites.wss/zz/en/?pageType=page&c=J179530Z42409M36

* [Mobile Application Developer skills for IBM MobileFirst Platform Foundation](https://www-304.ibm.com/services/learning/pdfs/mobile_ad.pdf)

## Download
* [Download](https://mobilefirstplatform.ibmcloud.com/downloads/)


## Documentation
* [Documentation](https://www.ibm.com/support/knowledgecenter/SSHS8R_7.1.0/wl_welcome.html)
* 


## Introduction to MobileFirst Studio
IBM MobileFirst Platform Studio is an Eclipse plug-in that supports the development of rich, mobile web, native, and hybrid apps. It contains an embedded version of MobileFirst Server, a bidirectional WYSIWYG editor, and standard web technologies and tools.

You use MobileFirst Studio to:

* Develop rich HTML5, hybrid and native applications for all supported modern devices
* Maximize code sharing by defining custom behavior and styling guidelines that match the target environment
* Access device APIs by using native code or standard web languages over a uniform Apache Cordova bridge
* Preview and manage applications by using MobileFirst Console
* Create custom server-side Java code that can be used by MobileFirst adapters
* Create, modify and test MobileFirst Java and JavaScript adapters
* Use both native and standard web languages within the same application to achieve development efficiency and provide a rich user experience
* Use third-party tools, libraries, and frameworks

## Introduction to MobileFirst CLI
IBM MobileFirst Platform Foundation provides a command-line interface tool to easily create and manage apps. The CLI lets you use your preferred text editors or alternative IDEs to create mobile applications.

The commands support tasks such as creating, adding, and configuring with the API library, adding the client-side properties file and performing the build and deploy of the application. From the command-line, you can create and deploy adapters, and test them locally. You can administer your project from CLI or REST services, or the Console, where you can control the local server and observe the logs.



##Tutorial
*[Tutorial](https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/all-tutorials/)


http://event.on24.com/clients/ibm/mobilefirst/build.html?


MobileFirst Platform Foundation

MobileFirst Quality Assurance

Cloudant Data Layer

MobileFirst Application Scanning

Presence Insights



https://mobilefirstplatform.ibmcloud.com/labs/


The following applications are used throughout the lab sessions for developers.

HybridWallet
MobileFirst Platform Foundation 7.1 application. Based on Ionic framework.
canteenPOS
MobileFirst Platform Foundation 7.1 application. Based on Ionic framework.
MFPcomradePOT
MobileFirst Platform Foundation 7.1 application. Based on Ionic framework.
Hello Paris
MobileFirst Platform Foundation 7.0 application. Based on Ionic framework.
More apps: (these apps are not supported)

IBM ReadyApps



Offline Reading
https://github.com/MobileFirst-Platform-Developer-Center/TutorialsForOfflineReading/tree/release80


https://mobilefirstplatform.ibmcloud.com/downloads/

http://www.slideshare.net/ibmmobilefirst/ibm-mobilefirst-technical-overview

https://dzone.com/articles/getting-started-with-ibm-mobilefirst

http://www.tricedesigns.com/2014/12/31/unified-multi-platform-push-notifications-with-ibm-mobilefirst/

https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/all-tutorials/

https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/setting-up-your-development-environment/setting-up-the-mobilefirst-development-environment/

https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/7.1/all-tutorials/

http://www.ibm.com/mobilefirst/us/en/downloads/

http://www-01.ibm.com/support/docview.wss?uid=swg24040199

https://www.ibm.com/support/knowledgecenter/SSHS8R_7.1.0/wl_welcome.html

https://github.com/MobileFirst-Platform-Developer-Center/TutorialsForOfflineReading/tree/release80

http://searchmobilecomputing.techtarget.com/definition/IBM-MobileFirst-Platform

http://blog.ionic.io/ionic-creator-available-for-ibm-mobilefirst-platform-users/

https://mobilefirstplatform.ibmcloud.com/tutorials/en/foundation/6.3/advanced-topics/shell-development-concepts/

http://www.exitcertified.com/training/ibm/websphere/application-development/native-app-development-mobilefirst-platform-foundation-ios-byoe-43622-detail.html

http://searchsoftwarequality.techtarget.com/feature/Breaking-down-IBMs-MobileFirst-Platform-Foundation

http://searchmobilecomputing.techtarget.com/feature/Understanding-IBMs-MobileFirst-Platform
http://asmarterplanet.com/mobile-enterprise/blog/2015/02/getting-started-ibm-mobilefirst-mobile-platform.html


