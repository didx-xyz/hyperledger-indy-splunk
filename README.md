# hyperledger-indy-splunk
Splunk App to monitor health and metrics for Hyperledger Indy networks.

The outputs from the https://github.com/bcgov/indy-node-monitor repo will be used to feed the Splunk app to enable metrics to be collected from Hyperledger Indy networks.

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
