# facedrive-docs
## How does it works?
1. Checkout the `development` branch
2. cd to : `pom.xml`, change active profile: 
```
        <profile>
            <id>stage</id>
            <activation>
                <activeByDefault>true</activeByDefault>
            </activation>
            <properties>
                <profile.resources>resources-stage</profile.resources>
            </properties>
        </profile>
```
3. Run with Spring boot, then check the `server.port` in the `resource-${profile}/env.properties`

