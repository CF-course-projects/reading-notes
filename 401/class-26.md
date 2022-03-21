# Android Fundamenals

## App fundamentals
- Androids apps can be written in Kotlin, Java, and C++
- An Android package is an archive file with an .apk suffix, containing of an Android app that are required at runtime.
- An Android app bundle, an archive file with an .aab suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime.

- The Android operating system is a multi-user Linux system in which each app is a different user.
- By default the systen assigns each app a unique Linux user ID (The Id is only known to the system and unknown to the app). The system sets permissions for all the files in the app so that only the user ID assigned to the app can access them
- An app's code runs in isolation from other apps; each process has its own virtual machine (VM)

### Principle of least privilege
- Each app has access only to the componenets that it requires to do its work and no more.
  - This means that apps are encapsulated within their own functionalities
  - Two apps CAN share the same Linux user ID, in which case they can access each other's files.
    - To conserve system resources, app with the same user ID can share the same VM
    - An app can request permission to access the device data, but the user has to explicitly grant these permissions.

### App components
- App components are the building blocks of an Android app. Each component is an entry point into your app for the system/user
- There are 4 types of components:
  - Activities
  - Services
  - Broadcast receivers
  - Content providers

#### Activities
- An activity is the entry point for interacting with the user: It is a single screen with a user interface
- Each activity is independent of others
- An activity facilitates key interaction between system and app
  - Keeping track of what is on the user's screen to ensure that the system keeps running the process that is hosting the activity
  - Knowing the previously used processses contain things the user may return to, and thus more highly prioritize keeping those processes around.
  - Helping the app handle having its processes killed so that the user can reutrn to activities with their previous state restored.
- You implement an activity as a subclass of the Activity class. 

#### Services
- A service is a general purpose entry point for keeping an app running in the background.
- A service does NOT provide a user interface
- Two types of services: 
  - **Started services**: tell the system to keep them running until their work is completed. 
    - Serives that the user is directly aware of (like music playing) are prioritized as the user will be unhappy if they are suddenly terminated
    - Regular background services are those of which the user is not directly aware of (think data syncing etc) and can be killed if necessary and restarted later if RAM needs to be reallocated
  - **Bound services**: run as API's for other processes. If process A calls upon process B, process B is bound to A when A is running.
  - Due to the flexibility of services, they are the basis of live wallpapers, notifications listners, screen savers, input methods etc
- A service is implemented as a subclass of service

#### Broadcast receivers
- A broadcast receiver is a component that enalbes the system to deliver events to the app outside of regular user flow, allows the app to respond to system-wide broadcast announcements
- The system can deliver broadcasts to apps that are not currently running
- More commonly, broadcast receivers are used as gateways to components and is intented to do a very minimal amount of work
- A broadcast receiver is implemented as a subclass of BroadcastReceiver and each broadcast is delivered as an Intent object.

#### Content providers
- A content provider manages a shared set of app data that you can store in the file system, in a SQLite database
- Using the content provider, apps can query or modify the data if the content provider allows it.
- To the system, a content provider is an entry point into an app for publishing named data items, identified by a URI scheme.
  - An app can define how it wants to map its data to a URI namespace, passing those URIs to other entities which can use them to access the data
  - Assigning a URI doesn't require that the app remain running; URIs can persist after their owning apps have exited. To retrieve the app's data from a URI, the corresponding owning app must be running
- A content provider is implemented as a subclass of of ContentProvider and must implement a standard set of APIs taht enable other apps to perform transcations.


