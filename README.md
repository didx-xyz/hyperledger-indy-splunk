# Splunk App for Hyperledger Indy

Hyperledger Indy app for Splunk offers an option to visualize _Hyperledger Indy_ metrics data. Splunk Indy helps you to gain deeper security and operational visibility into a Hyperledger Indy infrastructure by monitoring Hyperledger Indy network nodes.
* * *

### Documentation

- TBD

## Branches

- `master` branch contains the latest code, be aware of possible bugs on this branch.

### Prerequisites
1. Use the [fetch_monitor.py](https://github.com/hyperledger/indy-node-monitor/blob/master/fetch-validator-status/fetch_status.py) script from the [indy-node-monitor](https://github.com/hyperledger/indy-node-monitor) repository to fetch data from indy networks

1a. You will require a `NETWORK_MONITOR` DID on the associated Indy Network to extract detailed and status information from the [fetch_monitor.py](https://github.com/hyperledger/indy-node-monitor/blob/master/fetch-validator-status/fetch_status.py) script.
Anonymous information can be extracted as per the example in 1d. below.
   
1b. An example `cron` job to fetch detailed validator info every ten minutes ``*/10 * * * * root /home/splunk/indy-node-monitor/fetch-validator-status/run.sh --net=smn --seed=<NETWORK_MONITOR DID SEED> > /home/splunk/indy_ledgers_data/mainnet/`date "+\%Y-\%m-\%d_\%H:\%M:\%S"`_mainnet_detailed.json``

1c. An example `cron` job to fetch status validator info every ten minutes ``*/10 * * * * root /home/splunk/indy-node-monitor/fetch-validator-status/run.sh --net=smn --status --seed=<NETWORK_MONITOR DID SEED> > /home/splunk/indy_ledgers_data/mainnet/`date "+\%Y-\%m-\%d_\%H:\%M:\%S"`_mainnet_status.json``

1d. An example `cron` job to fetch anonymous validator info every ten minutes ``*/10 * * * * root /home/splunk/indy-node-monitor/fetch-validator-status/run.sh --net=smn --anonymous > /home/splunk/indy_ledgers_data/mainnet/`date "+\%Y-\%m-\%d_\%H:\%M:\%S"`_mainnet_anon.json``

2. At least one __Splunk Enterprise indexer__.
3. Create a Splunk index called `indy`
4. Install the `TA_hyperledger_indy` and `SA-Hyperledger-Indy` apps
5. Configure path in [inputs.conf](SA-Hyperledger-Indy/local/inputs.conf) to match your ledger data location
6. Restart splunk
7. Access the Splunk `Hyperledger Indy App`

## Installation

| Splunk version | Splunk Indy version     | Installation                                                   |
| :------------: | :---------------: | :--------------------------------------------------------------|
|      8     |       1.0.0       | <xyz> |

## Contribute

If you want to contribute to our project please don't hesitate to send a pull request. 
You can also join [DIDx Slack](https://join.slack.com/t/didx-xyz/shared_invite/zt-madh6xua-TzkbEWmqRhhFvag8WUPUxQ) to ask questions and participate in discussions.

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

-   [Hyperledger Indy](https://www.hyperledger.org/use/hyperledger-indy)
-   [Splunk documentation](http://docs.splunk.com/Documentation)
