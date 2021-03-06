---
title: "Snapcast"
description: "Instructions on how to integrate Snapcast into Home Assistant."
logo: snapcast.png
ha_category:
  - Media Player
ha_release: 0.13
ha_iot_class: Local Polling
redirect_from:
 - /components/media_player.snapcast/
---

The `snapcast` platform allows you to control [Snapcast](https://github.com/badaix/snapcast) from Home Assistant.

To add Snapcast to your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
media_player:
  - platform: snapcast
    host: YOUR_IP_ADDRESS
```

{% configuration %}
host:
  description: The IP address of the device, e.g., `192.168.0.10`.
  required: true
  type: string
port:
  description: The port number.
  required: false
  default: 1705
  type: integer
{% endconfiguration %}
