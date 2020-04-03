# MqttBridge

[![Continous Integration](https://gitlab.com/project-alice-assistant/skills/skill_MqttBridge/badges/master/pipeline.svg)](https://gitlab.com/project-alice-assistant/skills/skill_MqttBridge/pipelines/latest)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=project-alice-assistant_skill_MqttBridge&metric=alert_status)](https://sonarcloud.io/dashboard?id=project-alice-assistant_skill_MqttBridge)

bridge events between alice and mqtt.
All events that are shared with skills will create the following MQTT Message:
```
projectalice/events/<eventName>/<eventArguments>
```
the event arguments are a string converted dict, with the structure:
```
'{
	"<argumentName>": <value>,
	...
}'
```

- Author: maxbachmann
- Maintainers: N/A
- Alice minimum Version: 1.0.0-a5
- Requirements: N/A

