Go Plugin Samples:
==================
This is set of plugin samples to be used with Go-server.
Samples are provided with the intention of helping a plugin developer kick-start in a faster way. This sample is a maven project.

From Go version 14.4.0 Plugin implementation has changed from API based plugin to JSON based plugin.
While we recommend writing all new plugins using the JSON based extension, the older API based plugin implementation will continue to exist for a few more releases.

The sample implementation for JSON based extension can be found under 'curl-plugin' folder. However, if you want to refer to the old API based implementation, you can refer the folder under 'curl-plugin-old-api-based'.

Following are steps to be followed to get started with the samples

All Go plugins needed to depend on Go plugin API jar. To get started, get a copy of API jar and place it inside some folder.

1. Sample plugins use maven for dependency resolution. The Go plugin API jar is now available through Maven central.

2. Run mvn clean install - this would build the plugins. Jars would be available in the 'target' folder of individual modules.

3. Copy these built jar files onto your Go Server's external plugins directory and restart the Go Server.

4. The Plugins tab under the Go server Administration will list the plugins installed and you should see the installed samples in the list.

5. You could open the project using the pom.xml in any IDE of your choice and play around with the code.
   Note: Once Go plugin API is installed to maven repo, there should be no errors related to plugin API.

For more information on building Go plugins, visit: https://developer.gocd.org/current/writing_go_plugins/overview.html

## License

```plain
Copyright 2017 ThoughtWorks, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
