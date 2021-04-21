## by viewmodels() not work

```
    // necessary for viewmodels()
    implementation "androidx.activity:activity-ktx:$rootProject.activity_version"
    implementation "androidx.fragment:fragment-ktx:$rootProject.fragment_version"
```

## Failed when access internet
java.net.SocketException: Socket failed: EPERM(Operation not permitted)

Solution: Unistall the app and reinstall it
This may be caused because you forgot declaring the permission.
