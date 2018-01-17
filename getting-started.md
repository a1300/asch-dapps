

# Asch-Dapp


#### Folder structure & installation
```
root  
     / asch-cli
     / asch-node-1
     / asch-node-2

# first install nvm
sudo apt-get install nvm
nvm install 7
nvm install 8

# create asch-cli
git clone https://github.com/aschplatform/asch-cli.git asch-cli && cd asch-cli && npm install && chmod u+x bin/asch-cli && nvm use 8 && bin/asch-cli -help && cd ..


# create asch-node-1
git clone https://github.com/aschplatform/asch.git asch-node-1 && cd asch-node-1 && npm install && nvm use 7 && cd ..
# start the first node:
nvm use 7
cd asch-node-1
node ./app.js
cd ..


# create asch-node-2
git clone https://github.com/aschplatform/asch.git asch-node-2 && cd asch-node-2 && npm install && nvm use 7 && cd ..
# start the second node:
nvm use 7
cd asch-node-2
cd node ./app.js
```




#### Owner Address
```
address: A4hSa28WuATzkRiFDCsSpE8yvG9Py73uD1
secret: fall destroy discover turkey bronze smooth web grass slide vote wise sustain
publicKey: 47d16dbb8455142df6ba229b09f8c4b4056f75a49cb1c87d487bca728486e4d6
```

#### Create new  Dapp on localnet

```
# first start the first node (under point installation)
# start a new console
cd asch-node-1/dapps
nvm use 8

../../asch-cli/bin/asch-cli -H 127.0.0.1 dapps -a

# link to dapp.code?
https://github.com/sqfasd/asch-hello-dapp/archive/master.zip

# link to image?
http://1000logos.net/wp-content/uploads/2016/10/Bluetooth-Logo.png

# app-delegates (at least 5, look at appendix):


```

Hint to asch-cli: asch-cli error message not really helpful if not enough


#### Register Dapp on localnet
First you have to transfer money to your account to be able to register the dapp. Our main account is the **Owner Account** on the top of the document.

**Prerequesists**
- First node must run
- You are located in the ``root`` Folder
- For the parameter **secret** use the secret of a delegate located in ``asch-node-1/config.json``

```
# send money to our Owner-Address
nvm use 8
asch-cli/bin/asch-cli -H sendmoney --secret "" --to "A4hSa28WuATzkRiFDCsSpE8yvG9Py73uD1" --amount xxx
```






#### Register Dapp on localnet
Register Dapp with the secret of our **Owner Account**
Current directory ``asch-node-1/dapps``
```
nvm use 8
../../asch-cli -H 127.0.0.1 registerdapp --metafile dapp.json --secret "fall destroy discover turkey bronze smooth web grass slide vote wise sustain"
```



-----------------------------
-----------------------------
-----------------------------



# Appendix

### asch-dapp-1/config.json
First node is configured on port 4096 on localhost (127.0.0.1)
```
{
  "port": 4096,
  "address": "localhost",
  "publicIp": "",
  "logLevel": "debug",
  "magic": "594fe0f3",
  "api": {
    "access": {
      "whiteList": []
    }
  },
  "peers": {
    "list": [
      {
        "ip": "127.0.0.1",
        "port": 5000,
        "state": 2,
        "os": "linux3.13.0-87-generic",
        "version": "1.3.5"
      }
    ],
    "blackList": [],
    "options": {
      "timeout": 4000
    }
  },
  "forging": {
    "secret": [
      "aware rabbit syrup expose visa list pause shuffle lunch audit exchange wrong",
      "early sugar cannon mansion expose tunnel piece manual destroy exhaust helmet rather",
      "alter art sick gallery equal voice bunker sauce claw tourist twice essay",
      "pigeon chalk mother east harbor enlist busy parrot dune humble faith thought",
      "raise cloud royal wonder cradle job gate wife depth device bitter hope",
      "quarter predict civil guide attend chunk negative wheel rapid arm unfair rookie",
      "ceiling hair stick remember school agree reunion typical before ridge shy laugh",
      "steak turn suffer banner hope pretty angle exclude leg betray matter sweet",
      "regular eagle edge voice armor job purity alter genre soap embark chapter",
      "rubber paper menu pony able gather upon leaf pill pipe peace mad",
      "oil dawn illegal sea dish fashion frame goat render kidney unveil piece",
      "damp fortune lock reflect question roast dog clap wagon twist west life",
      "despair valley sunny junior text extra tooth cram lawn length any foot",
      "first depend endless coral wink square hockey oak october mercy warm step",
      "effort arch empower lucky normal cat split chest chat document thrive flame",
      "copy athlete latin know legend you air bitter apology valve replace alien",
      "bid face select across timber actor column ice chef retire plate unit",
      "slender mom bundle legend choose kingdom question shift into lazy public night",
      "echo eye crowd metal motor neither input phone person garlic six first",
      "visa real reopen veteran hill kick old hat resemble tobacco bracket sniff",
      "summer hundred fury used estate during flash planet sauce gentle sock enjoy",
      "improve food swim unaware clarify choice faint fossil foam cupboard random peasant",
      "horn boy win rifle enter ugly elevator sudden clarify quit float office",
      "warm zoo toast fit potato venue glory wedding skate era curtain diagram",
      "nuclear number adjust radio issue space squeeze frog guitar swear wife amused",
      "agent toss various salmon confirm avocado speed loyal december fantasy dilemma gold",
      "forward other chase wear regular harvest lyrics soldier circle hold frequent fade",
      "swing conduct situate ready chief glad mixed stumble soul chalk sorry chef",
      "side fossil account place sausage lady trouble patient flight random track bounce",
      "future program bubble cream man pyramid panic view around decrease daughter term",
      "climb assist forget raccoon mix engage swamp life glide brand public salt",
      "rail try above bitter indoor transfer acquire myth roof hammer kid appear",
      "engine paper bounce medal pulp napkin vintage metal olive bag candy system",
      "urge gold code spatial ship slam ridge put inside valley once stomach",
      "march essay agree rain error educate toward scout obey visa base suspect",
      "awake aerobic tenant grass include moon age program skin split wave finish",
      "unlock burden very exile unhappy plate upgrade among age sauce hen park",
      "staff usual more journey bomb addict wage tonight inflict scan cruise focus",
      "kitten season onion feel clever praise woman bring master fossil token school",
      "output awful spawn vacuum alarm wash toy busy frost dream eyebrow taxi",
      "tomato evolve turn desk slush dish volume daring crime pistol original diet",
      "chef useless worth sure reject upgrade rich real salad whale small sell",
      "cabbage force awake waste pelican bridge lobster announce jealous slow vibrant theory",
      "squirrel always urge audit subject upon connect embark juice gravity item cargo",
      "car know dragon congress whisper way famous truth island sphere fix history",
      "weather open buffalo love siren museum vehicle frog apple spy believe mother",
      "split diamond medal eyebrow license staff fluid dance rib bag bounce connect",
      "lawn emerge stadium monitor true alone cost just kingdom humble repeat pill",
      "impose guard wrist find clog hamster settle face resist essay legend follow",
      "destroy client brown cancel spoon left option demand skirt market funny mouse",
      "there provide dance eagle panda position swamp good fish coin fiction harvest",
      "winter front modify entire list clinic suggest zebra scan use mixture portion",
      "goose assist point staff valid crush audit settle involve silent load screen",
      "sign cactus protect help rich prevent indicate hurt screen donor acquire just",
      "crash unhappy salute quit exact horse jealous social goose pave useful alley",
      "grape crash unhappy spring tattoo traffic trick busy know detect cargo talent",
      "tube figure gown pulp garden ordinary case glue opinion wing occur cabin",
      "tissue north special grab artist office frequent view airport correct weather glove",
      "evidence main truth local album wrestle where dust glass dirt neither airport",
      "puzzle hungry surround permit since thumb hole shy hungry chest person banner",
      "twice sketch pilot hurt supreme crew such dove addict aunt blade bronze",
      "purchase focus dynamic few badge own replace gap bottom provide pistol minute",
      "nominee ring orient unusual major beach imitate nominee polar clip tree elephant",
      "pistol hunt twelve okay next lion sketch output exercise cushion holiday basic",
      "cabbage pause link old airport warm thank item shrug light doctor urge",
      "siege limit game space random nephew arrow gown toilet plunge weather endorse",
      "dad radio truth dynamic bounce tackle stumble grass give tackle ill ability",
      "jeans chair grow friend door siren rate setup mother oven double rabbit",
      "banner dash copy double alley enhance mystery rubber auto rice pencil jaguar",
      "process lawsuit heart ready exhibit average ripple eager era organ scrub candy",
      "elder suggest clerk mule gospel frost argue harbor announce become between attract",
      "decline leisure six spoil battle rhythm hurt keen rabbit network material brown",
      "tail ostrich snack ecology still belt useful segment fiscal entry tornado clog",
      "hip treat erosion owner festival engage lava wood creek walk boss right",
      "visual shrimp moment toilet purchase true repeat title attract verb toy cool",
      "woman shrug old auction peace auto detect wrist yellow peasant pretty waste",
      "burger virtual obey phone around garden thunder account great aisle hazard alert",
      "carbon flight pole spike bacon law arctic about before person electric diamond",
      "joy across crisp bone police coral define canoe weekend public palace camera",
      "sudden sure crystal offer pair judge dress panther minimum air title bid",
      "fetch top lens angle cliff clever will powder piece mind dad brick",
      "sponsor dinosaur feed absorb engage bubble success saddle song tilt giraffe car",
      "food select advance rotate sick much prosper senior lamp giraffe bar bubble",
      "fat domain run damp jump pool knife medal agree sample receive siege",
      "pact write imitate disagree pink shy crash clip employ wild twice fuel",
      "gadget ancient nest marine boost total quarter cable casual anxiety proof regret",
      "wave bread drill time apart bar negative ticket ensure gown depend fringe",
      "bone lawn tomato initial brisk opinion tiny arm nut immense wood floor",
      "pioneer ask eternal one copper aim firm extend harbor social cloud market",
      "where load ketchup arch topple excuse veteran present animal music permit virtual",
      "exist doll fitness witness annual tackle poverty olive have core canoe exhibit",
      "harvest horror normal globe very spend have soup face kidney flavor powder",
      "develop violin mutual once myth jar surface maximum refuse stock virtual glue",
      "purchase parade holiday custom strategy hood luxury cook call patrol total frozen",
      "saddle garbage benefit goddess lawsuit holiday entire wine pool orphan various impact",
      "sell west bridge neither firm glow skin effort announce notice point angle",
      "example goddess blame easily green auction joke bounce fix reject search uphold",
      "joke man canoe barrel machine captain obtain finish steel title portion power",
      "black camp change plastic consider calm ticket online cloud actual solve coach",
      "ability display fat question explain assault organ month winner hockey palm curtain",
      "decorate riot average weasel aspect seven decide biology body wheel trick pulp"
    ],
    "access": {
      "whiteList": [
        "127.0.0.1"
      ]
    }
  },
  "loading": {
    "verifyOnLoading": false,
    "loadPerIteration": 5000
  },
  "ssl": {
    "enabled": false,
    "options": {
      "port": 443,
      "address": "0.0.0.0",
      "key": "./ssl/server.key",
      "cert": "./ssl/server.crt"
    }
  },
  "dapp": {
    "masterpassword": "ytfACAMegjrK",
    "params": {}
  }
}
```

### Asch-dapp-2/config.json
Second node is configured on port 5000 on localhost (127.0.0.1)
```
{
  "port": 5000,
  "address": "127.0.0.1",
  "publicIp": "",
  "logLevel": "debug",
  "magic": "594fe0f3",
  "api": {
    "access": {
      "whiteList": []
    }
  },
  "peers": {
    "list": [
      {
        "ip": "127.0.0.1",
        "port": 4096,
        "state": 2,
        "os": "linux3.13.0-87-generic",
        "version": "1.3.5"
      }
    ],
    "blackList": [],
    "options": {
      "timeout": 4000
    }
  },
  "forging": {
    "secret": [
      "decorate riot average weasel aspect seven decide biology body wheel trick pulp"
    ],
    "access": {
      "whiteList": [
        "127.0.0.1"
      ]
    }
  },
  "loading": {
    "verifyOnLoading": false,
    "loadPerIteration": 5000
  },
  "ssl": {
    "enabled": false,
    "options": {
      "port": 443,
      "address": "0.0.0.0",
      "key": "./ssl/server.key",
      "cert": "./ssl/server.crt"
    }
  },
  "dapp": {
    "masterpassword": "ytfACAMegjrK",
    "params": {}
  }
}
```


**App-Delegates (at least 5):**
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
```