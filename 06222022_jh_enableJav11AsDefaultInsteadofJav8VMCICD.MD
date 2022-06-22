```
Author: lightsavers
Created: 06222022
```

# Firewall Settings (Centos7 Guest)

Java 8 is being phased out by many CI/CD applications, including Jenkins. 
An upgrade from Java 8 to Java 11 is almost a necessity for CI/CD. 

# Sample Scenario

1. Power on the VM locally or in your public cloud provider

2. Logging with your username with sudo powers

3. Begin by updating the system

```
sudo yum update 
```

4. Check the current Java version

```
java -version  
```

5. Install the Java JDK 11 (comes with JRE included)

```
sudo yum install java-11-openjdk-devel
```

6. Change Java default from Java 8 to Java 11

```
sudo alternatives --config java  
```

7. Select the Java version you would like to use (assuming you want to keep all Java versions)

8. Done
