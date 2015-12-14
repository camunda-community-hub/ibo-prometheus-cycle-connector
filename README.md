# Ibo Prometheus Connector

### Configuration Snippet

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
