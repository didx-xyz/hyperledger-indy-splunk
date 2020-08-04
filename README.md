# Splunk app for Hyperledger Indy

Hyperledger Indy app for Splunk offers an option to visualize _Hyperledger Indy_ metrics data. Splunk Indy helps you to gain deeper security and operational visibility into a Hyperledger Indy infrastructure by monitoring Hyperledger Indy network nodes.
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

    Copyright (C) 2020 DIDx, PTY, LTD.
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
    
Find more information about this on the [LICENSE](LICENSE) file.

## References

-   [DIDx website](https://www.didx.xyz)
-   [Hyperledger Indy](https://www.hyperledger.org/use/hyperledger-indy)
-   [Splunk documentation](http://docs.splunk.com/Documentation)
