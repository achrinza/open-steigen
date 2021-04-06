<!--
  SPDX-FileCopyrightText: 2021 The Open Steigen Authors
  SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Pairing Process

Steigens support 2 pairing modes; "EZ" and "AP" mode, both of which only support conecting to a 2.4 GHz network.

These pairing modes are standard for Tuya-powered IoT devices, though "EZ Mode" has been deprecated due to security concerns.

## EZ Pairing Mode

**This pairing mode is considered insecure.**

The EZ pairing mode enables Wi-Fi configuration of the Steigen appliance without needing the user to temporarily switch to another Wi-Fi network.

The EZ pairing mode procedure is as follows:

1. Set the Steigen Wi-Fi module into a promiscuous listening mode
2. Wi-Fi credentials is keyed into the Steigen Home app by the user
3. Steigen Home app encodes Wi-Fi credentials into data length values
4. A sequence of broadcast IPv4 UDP packets are sent to the user's Wi-Fi access point
5. The UDP packets are sniffed by the Steigen appliance which decodes the data length to retrieve the Wi-Fi credentials.
6. The Steigen appliance connects to the user's Wi-Fi access point and continues communication from there.

This pairing process is considered insecure as nearby malicious actors can sniff the unencrypted UDP packets and decode the plaintext Wi-Fi credentials.

## References

- Tuya IoT and EZ Mode Pairing - https://www.elttam.com/blog/ez-mode-pairing/