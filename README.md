# Splunk app for Hyperledger Indy

Hyperledger Indy app for Splunk offers an option to visualize _Hyperledger Indy_ metrics data. Splunk Indy helps you to gain deeper security and operational visibility into your Hyperledger Indy infrastructure by monitoring Hyperledger Indy networks.
* * *

### Documentation

- TBD

## Branches

- `stable` branch on correspond to the last stable app version.
- `master` branch contains the latest code, be aware of possible bugs on this branch.

### Prerequisites
1. You will require a DID on the Indy Network you want to monitor with the appropriate permissions to execute the [fetch_monitor.py](https://github.com/bcgov/indy-node-monitor) script against the associated ledger.
2. At least one __Splunk Enterprise indexer__.

## Installation

| Splunk version | Splunk Indy version     | Installation                                                   |
| :------------: | :---------------: | :--------------------------------------------------------------|
|      8     |       1.0.0       | <xyz> |

## Upgrade

Remove the app using splunk plugin tool

    $SPLUNK_HOME/bin/splunk remove app SplunkAppForIndy

Install the app

     $SPLUNK_HOME/bin/splunk install app <last package file>

## Contribute

If you want to contribute to our project please don't hesitate to send a pull request. 
You can also join [Sovrin Rocketchat](https://chat.sovrin.org) to ask questions and participate in discussions.

## Copyright & License

Copyright (C) 2015-2019 DIDx, PTY LTD.

This program is free software; you can redistribute it and/or modify it under the terms of the Apache License 2.0 License.

Find more information about this on the [LICENSE](LICENSE) file.

## References

-   [DIDx website](https://www.didx.xyz)
-   [Hyperledger Indy](https://www.hyperledger.org/use/hyperledger-indy)
-   [Splunk documentation](http://docs.splunk.com/Documentation)
