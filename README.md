<!--
  SPDX-FileCopyrightText: 2021 The Open Steigen Authors
  SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Open Steigen

A monorepo consisting of documentation and implementations of the local communication protocol used by Steigen Automatic Laundry Systems.

> **Note:** There are 2 "ecosystems" of Steigen appliances; They are differentiated by their compatibility with either the Steigen Home or Steigen Connect mobile app. As of right now, only Steigen appliances that support the Steigen Home mobile app have been tested.

## Table of Contents

- [Tested Hardware & Firmware](#tested-hardware-&-firmware)
- [Documentation](#documentation)
- [FAQs](#faqs)
- [License](#license)

## Tested Hardware & Firmware

> **Call for action:** If you have a Steigen appliance that is not listed in the table below, please help populate the table below with a pull request, or file a new "Appliance Compatibility" issue in the the issue tracker.

The following documentation and implementations have been tested on the following Steigen hardware and firmware, and what local protocol version is being used:

<table>
  <thead>
    <tr>  
      <th>Hardware</th>
      <th>Main Module</th>
      <th>MCU Module</th>
      <th>Local Protocol (v3.0 / 3.3)</th>
      <th>Date</th>
      <th>Working?</th>
      <th>Tested By</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Solar</td>
      <td>3.1.4</td>
      <td>2.0.0</td>
      <td>v3.3</td>
      <td><time datetime="2020-04-04">4 April 2020</time></td>
      <td>Yes</td>
      <td><a href="https://github.com/achrinza">@achrinza</a></td>
    </tr>
  </tbody>
</table>

Even if the hardware or firmware combination is not listed, the documentation and implementations should still work. If you're encountering any issues, please open file a new "Appliance Compatibility" issue in the issue tracker.

## Documentation

The protocol documentation can be found under `docs`.

## FAQs

The FAQ is broken down into the different docs pages so that they won't be too long and on-topic.

- [Data Points](./docs/data-points#faq)

## License

Copyright (c) 2021 The Open Steigen Authors.

Code in this monorepo are licensed under MIT.

Documentation in this monorepo are licensed under CC BY-SA 4.0.