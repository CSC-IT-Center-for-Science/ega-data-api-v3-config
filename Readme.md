# EGA.Data.API.v3.CONFIG

This is a standalone Spring Configuration server. It is configured to run on port 8888. The correct URL to this service must be specified in all micro services using the configuration server.

There are no dependencies.

This service provides `application.properties` files to micro services using the configuration server. This allows for centralised configuration management for multiple micro services, and it removes any configuration files from the source code.

The `application.properties` files are configured to be stored in directory `"${HOME}/ngs_3/config"` on the server hosting the confoguration service. The name for the properties file of a micro servcice named `{app.name}` is `"{app.name}.properties"`

