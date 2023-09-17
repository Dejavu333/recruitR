# recruitR
```
using env variables to config microservices in a docker container
reason: to avoid hardcoding values in the code other option would be to use a config file (yaml, json, etc) as we do in quiz_service appsettings.json
but we have to mount the file in the container and we have to make sure the file is not exposed to the public we do it to stcik to the c# standard
in kubernetes we can use secrets to store sensitive data like passwords, api keys, etc and we can mount them in the container as env variables or 
configmaps (configmaps are not encrypted) we can also use vault to store secrets and mount them in the container as env variables or configmaps
```


```

serilogcould write directly to elastic search but that wouldnt be language agnostic since the other microservices are implemented in a different lang
```


```

dont assert the details too soon
use case is an object , we can write the code for it becasue we use programming languages that can abstract (controll object, ye confusing because of modelviewcontroller, we can call it interactor too)

use cases are all about atomation they are application specific business rules

they are also application independent business rules , like interest calculation that were done regardless of automation, we can do it without calculator dont we

we dont want these two to couple

interactor would be console.readline() or in another implementation server.listen()
```


```
folder by feature over folder by type
cohesion and coupling are yingyang
afferent and efferent coupling
domain is dependent on nothing as we 
go outside the hexagonal the who im dependant on is  increases 
cohesion is behaviour that belongs together

classes of the same feature tends to evolve together, they should stay together, use feature folders. Reduces cognitive load, easier testing, more scalable and maintainable. Less coupling, every feature can have fully different implementation 

folders:
addorder
addproduct
cancelorder

every feature had its own view,controller,service,repo,ds etc or other things if you choose different arch
```
