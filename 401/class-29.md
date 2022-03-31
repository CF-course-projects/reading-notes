# Room

## Overview Saving Data With Room
- The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite.

### Setup 
```
dependencies {
    def room_version = "2.4.2"

    implementation "androidx.room:room-runtime:$room_version"
    annotationProcessor "androidx.room:room-compiler:$room_version"
 ```
### Primary Components:
  - There are three major components in Room:
    - Database class: holds the database and serves as the main access point for the connection to 
    - 
