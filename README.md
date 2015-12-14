# Camunda Cycle Ibo Prometheus Connector

This is a Ibo Prometheus Connector for [camunda Cycle][1]. It contains the implementation of a connector which persists and synchronizes bmpn models between the a Ibo repository and another location, like a file repository.  

## How to use it?

1. Checkout the project with Git
2. Build the project with maven
3. Deploy the jar file to a cycle distribution (see [installation guide][3])
4. Update the `connector-configurations.xml` file
4. Start Cycle, goto Connectors and add a new Example Connector

## Configuration Snippet

```xml
<bean name="iboConnectorDefinition" class="org.camunda.bpm.cycle.entity.ConnectorConfiguration">
  <property name="name" value="Ibo Connector"/>
  <property name="connectorClass" value="org.camunda.bpm.cycle.connector.ibo.IboConnector"/>
  <property name="properties">
    <map>
      <entry key="iboBaseUrl" value=""></entry>
      <entry key="proxyUrl" value=""></entry>
      <entry key="proxyUsername" value=""></entry>
      <entry key="proxyPassword" value=""></entry>
    </map>
  </property>
</bean>
```

## Maintainers

[Ibo][4]

[1]: https://docs.camunda.org/manual/7.4/webapps/cycle/
[3]: https://docs.camunda.org/manual/7.4/installation/cycle/#add-connectors
[4]: https://ibo.de/
