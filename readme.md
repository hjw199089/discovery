
debug param
```
mainclass:io.airlift.discovery.server.DiscoveryServer
vm:-ea -XX:+UseG1GC -XX:G1HeapRegionSize=100M -XX:+UseGCOverheadLimit -XX:+ExplicitGCInvokesConcurrent -Xmx2G -Dconfig=/Users/xx/Documents/Codes/airlift_discovery/discovery/discovery-server/etc/config2.properties -Dlog.levels-file=/Users/xx/Documents/Codes/airlift_discovery/discovery/discovery-server/etc/log.properties
working directory:/Users/xx/Documents/Codes/airlift_discovery/discovery 
use classpath module:discovery-server
```

config2.properties

``
node.environment=test
http-server.http.port=8411
node.id=0BA42FDB-5DBA-4A2C-BE26-9596B7B4368E
service-inventory.uri=file:/Users/xx/Documents/Codes/airlift_discovery/discovery/discovery-server/etc/service-inventory.json
``

service-inventory.json

```
{
    "environment": "test",
    "services": [
        {
            "id": "C8A9EE64-0476-452C-8638-8E72F3EE3CA6",
            "nodeId": "597A741E-9968-40E2-BB4D-7AF26DE18689",
            "type": "discovery",
            "pool": "general",
            "location": "/localhost",
            "state": "RUNNING",
            "properties": {
                "http": "http://localhost:8411"
            }
        }
    ]
}

```
