# sample-springboot-config

This is a sample git repository used to demonstrate using the gitcontroller as described in the [Microservices configuration guide](http://fabric8.io/guide/develop/configuration.html#git)

If you run the [sample application](https://github.com/jstrachan/springboot-config-demo) it will have a [`gitRepo` volume to that mounts the application.properties file](https://github.com/jstrachan/springboot-config-demo/blob/master/src/main/fabric8/deployment.yml#L5-L14). 

Then as you edit this repository the `gitcontroller` should perform [rolling updates](http://kubernetes.io/docs/user-guide/rolling-updates/) to the [Deployment](http://kubernetes.io/docs/user-guide/deployments/) to use the new configuration values!
