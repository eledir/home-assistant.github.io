---
layout: page
title: "OctoPrint"
description: "Instructions how to setup the OctoPrint in Home Assistant."
date: 2015-01-20 22:36
sidebar: true
comments: false
sharing: true
footer: true
logo: octoprint.png
ha_category: Hub
featured: false
ha_release: 0.19
---

[OctoPrint](http://octoprint.org/) is a web interface for your 3D printer. This is the main component to integrate OctoPrint sensors, you will have to setup sensors and binary sensors separately.

To get started with the OctoPrint API, please follow the directions on their [site](http://docs.octoprint.org/en/master/api/general.html). Once OctoPrint is configured you will need to add your API key and host to your `configuration.yaml`. 


```yaml
octoprint:
  host: YOUR_OCTOPRINT_HOST
  api_key: YOUR_API_KEY
```

Configuration variables:

- **host** (*Required*): IP address or hostname of Octoprint host.
- **api_key** (*Required*): The retrieved api key.


**NOTE** If your 3D printer isn't connected to the OctoPrint server during the startup of Home Assistant this component will fail to load.
