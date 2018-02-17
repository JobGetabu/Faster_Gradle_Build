# Faster_Gradle_Build
this is tweak to increase android gradle build time by 65% tested :}

## Add the following line in gradle/properties file

### Enable daemon
org.gradle.daemon=true

### Try and findout the best heap size for your project build.
org.gradle.jvmargs=-Xmx3096m -XX:MaxPermSize=512m -XX:+HeapDumpOnOutOfMemoryError -Dfile.encoding=UTF-8

### Modularise your project and enable parallel build
org.gradle.parallel=true

### Enable configure on demand.
org.gradle.configureondemand=true
