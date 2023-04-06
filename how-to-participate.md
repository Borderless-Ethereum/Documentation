---
description: If you're a validator, this is how you can participate
---

# 🤝 How to Participate

This is a rough guide to describe how you as a validator node operator can participate in the project.  In order to participate, you need to configure the graffiti field in your consensus client of choice to include a geo-tag. Every client has a different way to configure the graffiti field and some clients are more configurable than others. Please refer to the document of your [respective client for more details](client-configuration.md).

In terms of what to add to the Graffiti field of your client, please refer to the the [list of ISO 3166-1 alpha-2 codes](list-of-country-codes.md) for the code for your respective country of operation. Take the two letter code and append it to the keyword “GEO”, such that it looks like “GEO-XX” where XX is the country code.

**Examples:**

* Estonia: GEO-EE
* India: GEO-IN
* El Salvador: GEO-SV

The geo-tag can be placed anywhere within the graffiti field so that it can be mixed with other graffiti field data, such as the client name and version, or [beaconcha.in](http://beaconcha.in) graffiti wall.
