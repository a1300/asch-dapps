

# Asch-Dapp


#### Folderstructure

```
dev  
     /asch-cli
       ...
     /asch
       ...
```



```
# Owner Address
address: A4hSa28WuATzkRiFDCsSpE8yvG9Py73uD1
secret: fall destroy discover turkey bronze smooth web grass slide vote wise sustain
publicKey: 47d16dbb8455142df6ba229b09f8c4b4056f75a49cb1c87d487bca728486e4d6
```

#### Create new  Dapp on localnet

```
nvm install 8.0.0
nvm use 8
```
(for asch-cli, asch-cli error message not really helpful)

#### Register Dapp on localnet

```
../../../asch-cli/bin/asch-cli -H 127.0.0.1 dapps -a

# link to dapp.code?
https://github.com/sqfasd/asch-hello-dapp/archive/master.zip

# link to image?
http://1000logos.net/wp-content/uploads/2016/10/Bluetooth-Logo.png

```


#### App-Delegates (at least 5):

```
# Delegate 1
address: AnHbLXumRfHyFV87CnTiGTcAES7hPwox8,
secret: pride emotion shiver prize before brief movie panda wrestle monkey custom smile
publicKey: 8c117a74efe93e64287ee54c4d424f4b61c3bf22dc6b6fcbe84c0a7f03c9da96

# Delegate 2
address: ALNnXxg3M5VZkuSc s1ZvGuEUtJmgQKY98X',
secret: country donate issue boring derive ketchup fish alarm acid disease shallow mirror
publicKey: 10e30ac04d83562727a686719227baff3265c5bb36d16da0edc0bb4c335776fc

# Delgate 3
address: ALixj31iCEfR8AnYU2TwXsLzSK8u8E4qc9
secret: era alcohol tiger style choice radio bike airport book limit harsh rubber
publicKey: 0b543d3cbd6355b26251ad66abe531eac1e620a2751945ee2ddbd80402a0d1cc

# Delegate 4
address: ANQDEYH2L3uairp5tCo1X6MQFk66Cx7unw
secret: inmate cabbage acoustic vote admit ahead salmon huge leaf pink reunion sun
publicKey: 0556397b30fda6b229b2c47448a5f7325ddfe146d4008f7ffef07414b0549b11

# Delgate 5
address: APCXr6AeoQZTfqzmfBC8E1U7h1fNN8GjCW
secret: rain organ hat zoo adjust fall dad crack fiction search grow reopen
publicKey: 93d9104c5d8a2c1a2593d241fab7e42e9df6da3e0ededf3078a1b080d86a38ad



#### TODO:
-XAS mit methode sendmoney (asch-cli) an den Owner der Dapp senden (weil registrieren etwas kostet)
send money for registration: ```asch-cli -H sendmoney --secret "" --to "" ```

register dapp on localnet: ```asch-cli -H 127.0.0.1 registerdapp --metafile dapp.json --secret "fall destroy discover turkey bronze smooth web grass slide vote wise sustain"```
