---
id: technical-faqs
title:
description:
keywords:
  - docs
  - matic
image: https://matic.network/banners/matic-network-16x9.png
---

###  {#1-are-the-private-keys-same-for-heimdall-and-bor-keystore}


###  {#2-list-of-common-commands}





####  {#a-where-to-find-heimdall-genesis-file}

`$CONFIGPATH/heimdall/config/genesis.json`

####  {#b-where-to-find-heimdall-config-toml}

`/etc/heimdall/config/heimdall-config.toml`

####  {#c-where-to-find-config-toml}

`/etc/heimdall/config/config.toml`

####  {#d-where-to-find-heimdall-seeds-txt}

`$CONFIGPATH/heimdall/heimdall-seeds.txt`

####  {#e-start-heimdall}

`$ sudo service heimdalld start`

####  {#f-start-heimdall-rest-server}

`$ sudo service heimdalld-rest-server start`

####  {#g-start-heimdall-bridge-server}

`$ sudo service heimdalld-bridge start`

####  {#h-heimdall-logs}

`/var/log/matic-logs/`

####  {#i-where-to-find-bor-genesis-file}

`$CONFIGPATH/bor/genesis.json`

####  {#j-start-bor}

`sudo service bor start`

####  {#k-check-heimdall-logs}

`tail -f heimdalld.log`

####  {#l-check-heimdall-rest-server}

`tail -f heimdalld-rest-server.log`

####  {#m-check-heimdall-bridge-logs}

`tail -f heimdalld-bridge.log`

####  {#n-check-bor-logs}

`tail -f bor.log`

####  {#o-kill-bor-process}



1.
2. `sudo kill -9 PID`





###  {#3-error-failed-to-unlock-account-0x-no-key-for-given-address-or-file}





1.



2.



3.



1.

`~/.bor/keystore/`

2.

`~/.bor/password.txt`


###  {#4-error-wrong-block-header-apphash-expected-xxxx}





```bash
    sudo service heimdalld stop

    heimdalld unsafe-reset-all
```



```bash
    wget -c <Snapshot URL>

    tar -xzvf <snapshot file> -C <HEIMDALL_DATA_DIRECTORY>

```




###  {#5-from-where-do-i-create-the-api-key}





###  {#6-heimdall-isn-t-working-i-m-getting-a-panic-error}






###  {#7-how-do-i-delete-remnants-of-heimdall-and-bor}





```$ sudo dpkg -i matic-bor```



```$ sudo rm -rf /etc/bor```



```$ sudo rm -rf /etc/bor```



```$ sudo rm /etc/heimdall```


###  {#8-how-many-validators-can-be-active-concurrently}



###  {#9-how-much-should-i-stake}











###  {#10-i-was-selected-to-become-a-validator-but-my-eth-address-was-incorrect-what-do-i-do}





###  {#11-i-m-getting-an-error-starting-the-bridge}








###  {#12-i-m-getting-dpkg-error}





`sudo dpkg -r matic-node`


###  {#13-i-m-not-clear-on-which-private-key-should-i-add-when-i-generate-validator-key}




###  {#14-is-there-a-way-to-know-if-heimdall-is-synced}



```$ curl [http://localhost:26657/status](http://localhost:26657/status)```




###  {#15-what-if-someone-become-a-top-10-staker-how-he-will-receive-his-matic-reward-at-the-end}




###  {#16-what-should-be-my-heimdall-version}



```heimdalld version```




###  {#17-what-values-should-i-add-in-the-stake-amount-and-fee-amount}









###




###  {#19-when-i-make-the-stake-transaction-i-m-getting-gas-exceeded-error}









###  {#20-when-will-i-get-a-chance-to-become-a-validator}




###  {#21-where-can-i-find-heimdall-account-info-location}








###  {#22-which-file-do-i-add-the-api-key-in}




###  {#23-which-file-do-i-add-the-persistent_peers}





###  {#24-did-you-reset-tendermint-without-resetting-your-application-s-data}





###  {#25-error-unable-to-unmarshall-config-error-1-error-s-decoding}





###  {#26-to-stop-heimdall-and-bor-services}







1.
2. `sudo kill -9 PID`









###  {#27-to-remove-heimdall-and-bor-directories}











###  {#28-what-to-do-when-you-get-wrong-block-header-apphash-error}

