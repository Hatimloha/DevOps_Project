# Address
- We have to copy and paste in every new firewall

> We have to copy and paste in every new firewall
```bash
config firewall address
    edit "all"
        set uuid 3a03c4da-2eee-51eb-c52e-1c3bd9078433
    next
    edit "FIREWALL_AUTH_PORTAL_ADDRESS"
        set uuid 3a03df38-2eee-51eb-66b6-20a2735fa4df
    next
    edit "FABRIC_DEVICE"
        set uuid 3a03faea-2eee-51eb-6017-f9b04a61633a
        set comment "IPv4 addresses of Fabric Devices."
    next
    edit "SSLVPN_TUNNEL_ADDR1"
        set uuid 6e4c0e0e-d198-51ea-e799-e421f3813e9d
        set type iprange
        set start-ip 10.212.134.200
        set end-ip 10.212.134.210
    next
    edit "IIHPLMIS"
        set uuid b2b21482-00ec-51ed-62d8-f7dc84e1fdee
        set type fqdn
        set fqdn "*.iihplmis.com"
    next
    edit "HDFC corporate"
        set uuid b2b59c24-00ec-51ed-f991-6c5309a1982e
        set type fqdn
        set fqdn "corporate.hdfcbank.com"
    next 
    edit "HIS-MAIN"
        set uuid b2b75d02-00ec-51ed-3e48-f2a893dc1807
        set type fqdn
        set fqdn "his.indiraivf.in"
    next 
    edit "HIS_TRAINING"
        set uuid b2b907b0-00ec-51ed-a9ad-3ad637915b05
        set type fqdn
        set fqdn "hmistraining.indiraivf.in"
    next 
    edit "JIRA"
        set uuid 0ee44478-c503-51ea-edbc-9351f26dc874
        set type fqdn
        set fqdn "indiraivf.atlassian.net"
    next 
    edit "Tikona_Server_1"
        set uuid f5fbe4b0-08c7-51ed-7e5a-ad6d0027d3c3
        set subnet 202.56.126.7 255.255.255.255
    next 
    edit "Tikona_Server_2"
        set uuid f5fe141a-08c7-51ed-28a4-2e445b6a66de
        set subnet 203.90.66.87 255.255.255.255
    next 
    edit "Tikona_Capstone_Server"
        set uuid f600c476-08c7-51ed-dfd9-7a8caa32339f
        set subnet 113.193.14.44 255.255.255.255
    next 
    edit "Udaipur"
        set uuid 28dfc8f2-db27-51ec-1e4a-ac3540ba5955
        set subnet 202.129.210.26 255.255.255.255
    next 
    edit "TallyServer1"
        set uuid b58b5eb8-2abb-51ed-de4e-d6f8c1437bb2
        set type fqdn
        set fqdn "v35131.22112.tallyprimecloud.in"
    next 
    edit "TallyServer2"
        set uuid b58bd9f6-2abb-51ed-5c87-d73efe290e75
        set type fqdn
        set fqdn "v35132.22112.tallyprimecloud.in"
    next 
    edit "M1"
        set uuid 5c2c13ae-4211-51ed-6528-b519deb3c359
        set type fqdn
        set fqdn "*.api.support.microsoft.com"
    next 
    edit "M2"
        set uuid 5c2c9a36-4211-51ed-5ef3-4cac591a018a
        set type fqdn
        set fqdn "*.aria.microsoft.com"
    next 
    edit "M3"
        set uuid 5c2cf4a4-4211-51ed-1e52-4e7393dd8dc2
        set type fqdn
        set fqdn "*.cc.skype.com"
    next 
    edit "M4"
        set uuid 5c2d4d78-4211-51ed-560d-509466c83cc4
        set type fqdn
        set fqdn "*.channelservices.microsoft.com"
    next 
    edit "M5"
        set uuid 5c2da67e-4211-51ed-bf84-f49ee5291a78
        set type fqdn
        set fqdn "*.channelwebsdks.azureedge.net"
    next 
    edit "M6"
        set uuid 5c2dfe26-4211-51ed-e591-a61988746b58
        set type fqdn
        set fqdn "*.edgeassetservice.azureedge.net"
    next 
    edit "M7"
        set uuid 5c2e5740-4211-51ed-9a5c-ef03615b191f
        set type fqdn
        set fqdn "*.flightproxy.skype.com"
    next 
    edit "M8"
        set uuid 5c2eb294-4211-51ed-4381-dcad9629ed53
        set type fqdn
        set fqdn "*.login.microsoftonline.com"
    next 
    edit "M9"
        set uuid 5c2f0dde-4211-51ed-989a-6f3469c50ae2
        set type fqdn
        set fqdn "*.monitor.azure.com"
    next 
    edit "M10"
        set uuid 5c2f6446-4211-51ed-a901-5d88fbaa8392
        set type fqdn
        set fqdn "*.registrar.skype.com"
    next 
    edit "M11"
        set uuid 5c2fbb08-4211-51ed-352b-29c08a235dda
        set type fqdn
        set fqdn "*.remoteassistanceprodacs.communication.azure.com"
    next 
    edit "M12"
        set uuid 5c3017a6-4211-51ed-382f-9cdfbdb6dedb
        set type fqdn
        set fqdn "*.support.services.microsoft.com"
    next 
    edit "M13"
        set uuid 5c30732c-4211-51ed-ab7e-22371b2cfc1d
        set type fqdn
        set fqdn "*.trouter.skype.com"
    next 
    edit "M14"
        set uuid 5c30cfac-4211-51ed-3ba2-68ff700d7574
        set type fqdn
        set fqdn "*.trouter.skype.com"
    next 
    edit "M15"
        set uuid 5c312916-4211-51ed-3a67-5ba8f11bdf9d
        set type fqdn
        set fqdn "*.turn.azure.com"
    next 
    edit "M16"
        set uuid 5c318406-4211-51ed-5af6-c351a18e66e7
        set type fqdn
        set fqdn "*.vortex.data.microsoft.com"
    next 
    edit "M17"
        set uuid 5c31e414-4211-51ed-4e10-0d387ee258a6
        set type fqdn
        set fqdn "browser.pipe.aria.microsoft.com"
    next 
    edit "M18"
        set uuid 5c32511a-4211-51ed-3116-e0b8be1c9e15
        set type fqdn
        set fqdn "edge.skype.com"
    next 
    edit "M19"
        set uuid 5c329eae-4211-51ed-b7c3-8f7b0bfa08d5
        set type fqdn
        set fqdn "events.data.microsoft.com"
    next 
    edit "ESHOPAID SERVER"
        set uuid cf5ede5e-4231-51ed-58d6-341f179032a5
        set type fqdn
        set fqdn "epos.indiraivf.in"
    next 
    edit "TrendMicro"
        set uuid 9fa604b0-0bf6-51ed-e6f2-925764d1a384
        set type fqdn
        set fqdn "osce14.icrc.trendmicro.com"
    next 
    edit "HRMAX"
        set uuid 265047b0-422e-51ed-279b-ac916b80e00b
        set type fqdn
        set fqdn "hrmax.myadrenalin.com"
    next 
    edit "p2p"
        set uuid 2650fa16-422e-51ed-06be-d02b2345da26
        set type fqdn
        set fqdn "xpa.indiraivf.in"
    next 
    edit "outlook"
        set uuid 2651a024-422e-51ed-7a5e-5b1508556ed2
        set type fqdn
        set fqdn "outlook.office365.com"
    next 
    edit "ms-teams"
        set uuid 2651f0a6-422e-51ed-85b1-9d3f2827394f
        set type fqdn
        set fqdn "teams.microsoft.com"
    next 
    edit "pinopen"
        set uuid b2b3dea2-00ec-51ed-2753-0e61eadbf28d
        set type fqdn
        set fqdn "www.pinopen.com"
    next 
    edit "NewsLetter"
        set uuid b2bacae6-00ec-51ed-17b8-157fc376e984
        set type fqdn
        set fqdn "indiraivftimes.eqtribe.com"
    next 
    edit "NewsLetter1"
        set uuid b2bc91e6-00ec-51ed-8e15-569da6b8bd3a
        set type fqdn
        set fqdn "eqplatform.eqtribe.com"
    next 
    edit "Eshop_server"
        set uuid b865150c-5536-51ed-c11c-85ee81c96342
        set subnet 3.109.19.78 255.255.255.255
    next 
    edit "P2P"
        set uuid b8670088-5536-51ed-39c9-73223e91a197
        set subnet 3.109.86.118 255.255.255.255
    next 
    edit "DLP-SERVER"
        set uuid 31395ce0-7855-51ed-3b03-01cb654d7e60
        set subnet 45.118.160.135 255.255.255.255
    next 
    edit "DT-PLUS"
        set uuid ccbe80ba-7b6f-51ed-3c5d-1082b2aae5d2
        set type fqdn
        set fqdn "www.drivetrackplus.com"
    next 
    edit "biometric emb lab"
        set uuid bbb560f0-92fc-51ed-5320-ba82c27ea370
        set subnet 192.168.1.15 255.255.255.255
    next 
    edit "paramount"
        set uuid 5452a39a-a149-51ed-b335-d23dce1ce988
        set type fqdn
        set fqdn "www.paramounttpa.com"
    next 
    edit "Gem-employease"
        set uuid 4bbfdb5a-a1ec-51ed-cb97-9aa493ff087f
        set type fqdn
        set fqdn "gem.employease.in"
    next 
    edit "HIS_TS"
        set uuid 677a98c2-f35a-51eb-1b88-b63be25b2f59
        set type fqdn
        set fqdn "his.indiraivf.in"
    next 
    edit "Tikona_NMS"
        set uuid 6f29133c-cefa-51ed-2f37-8c5337add05a
        set subnet 203.90.66.83 255.255.255.255
    next 
    edit "Udaipur-Ishan"
        set uuid 52b075ca-cd4b-51ed-5cb1-7dd4b409fde9
        set subnet 202.129.210.26 255.255.255.255
    next 
    edit "Udaipur-Airtel"
        set uuid 52b2a2f0-cd4b-51ed-1242-3a60bc62349c
        set subnet 122.185.53.90 255.255.255.255
    next 
    edit "Udaipur-Vodafone"
        set uuid 52b4df34-cd4b-51ed-26b0-f51981503d7b
        set subnet 123.63.187.130 255.255.255.255
    next 
    edit "Udaipur-Tata"
        set uuid 52b73e96-cd4b-51ed-a7c5-49813f2cce22
        set subnet 14.99.199.170 255.255.255.255
    next 
    edit "Mumbai-Primenet"
        set uuid 52b9c8d2-cd4b-51ed-df9a-8fe81623d40a
        set subnet 110.173.183.226 255.255.255.255
    next 
    edit "FMG-IP"
        set uuid 52bc28e8-cd4b-51ed-f78c-17aefe6c4501
        set subnet 199.34.20.228 255.255.255.255
    next 
    edit "FAZ-IP"
        set uuid 52be898a-cd4b-51ed-9a1e-b5c404b1b1a8
        set subnet 199.34.20.227 255.255.255.255
    next 
    edit "FCTEMS_ALL_FORTICLOUD_SERVERS"
        set uuid f18e76a0-d49f-51ed-628e-06b9bfd3280f
        set type dynamic
        set sub-type ems-tag
    next 
    edit "HARMFUL-IP1"
        set uuid e3f96ef8-d6d6-51ed-945c-5c137cc9ebc0
        set subnet 101.167.152.76 255.255.255.255
    next 
    edit "HARMFUL-IP2"
        set uuid e3fa6506-d6d6-51ed-f06f-e417057801d7
        set subnet 101.167.152.90 255.255.255.255
    next 
    edit "HARMFUL-IP3"
        set uuid e3fb150a-d6d6-51ed-8d88-8deec03233ac
        set subnet 109.235.139.13 255.255.255.255
    next 
    edit "HARMFUL-IP4"
        set uuid e3fbc392-d6d6-51ed-b7e1-8b2bda8e0fb8
        set subnet 213.61.253.152 255.255.255.255
    next 
    edit "HARMFUL-IP5"
        set uuid e3fc709e-d6d6-51ed-4b25-30b4adf8bc01
        set subnet 213.61.253.250 255.255.255.255
    next 
    edit "HARMFUL-IP6"
        set uuid e3fd24d0-d6d6-51ed-ac39-f7f89bb9b25a
        set subnet 213.61.254.11 255.255.255.255
    next 
    edit "HARMFUL-IP7"
        set uuid e3fdd146-d6d6-51ed-8f30-ebbe6d75f1ad
        set subnet 213.61.254.36 255.255.255.255
    next 
    edit "HARMFUL-IP8"
        set uuid e3fe81fe-d6d6-51ed-4a48-53429b96e539
        set subnet 217.110.80.14 255.255.255.255
    next 
    edit "HARMFUL-IP9"
        set uuid e3ff38c4-d6d6-51ed-41e6-79491d6537f5
        set subnet 138.68.190.172 255.255.255.255
    next 
    edit "HARMFUL-IP10"
        set uuid e3ffe2c4-d6d6-51ed-fadf-cf0d9d5b1cfc
        set subnet 172.104.154.229 255.255.255.255
    next 
    edit "HARMFUL-IP11"
        set uuid e4008b84-d6d6-51ed-61e9-02063b1e6de7
        set subnet 38.242.195.61 255.255.255.255
    next 
    edit "HARMFUL-IP12"
        set uuid e401373c-d6d6-51ed-84bd-c6ebd985c564
        set subnet 64.90.48.215 255.255.255.255
    next 
    edit "HARMFUL-IP13"
        set uuid e401e1b4-d6d6-51ed-25f6-7b43b41fcce9
        set subnet 5.189.159.215 255.255.255.255
    next 
    edit "HARMFUL-IP14"
        set uuid e4028a7e-d6d6-51ed-3578-e627307262b3
        set subnet 176.31.182.123 255.255.255.255
    next 
    edit "HARMFUL-IP15"
        set uuid e40334f6-d6d6-51ed-eec0-a5da5be64644
        set subnet 87.251.67.9 255.255.255.255
    next 
    edit "HARMFUL-IP16"
        set uuid e403e5b8-d6d6-51ed-8957-01c37dc94c7a
        set subnet 101.167.152.76 255.255.255.255
    next 
    edit "HARMFUL-IP17"
        set uuid e4049468-d6d6-51ed-b160-737d867912f2
        set subnet 101.167.152.90 255.255.255.255
    next 
    edit "HARMFUL-IP18"
        set uuid e4053f94-d6d6-51ed-31b4-c0215a09019a
        set subnet 109.235.139.13 255.255.255.255
    next 
    edit "HARMFUL-IP19"
        set uuid e405eafc-d6d6-51ed-b47e-1c56871696c8
        set subnet 213.61.253.152 255.255.255.255
    next 
    edit "HARMFUL-IP20"
        set uuid e40695c4-d6d6-51ed-903a-864887483e1c
        set subnet 213.61.253.250 255.255.255.255
    next 
    edit "HARMFUL-IP21"
        set uuid e4073ea2-d6d6-51ed-34eb-943f9dabb6dd
        set subnet 213.61.254.11 255.255.255.255
    next 
    edit "HARMFUL-IP22"
        set uuid e407f4fa-d6d6-51ed-bbdb-9b43b1b1b144
        set subnet 213.61.254.36 255.255.255.255
    next 
    edit "HARMFUL-IP23"
        set uuid e4089f68-d6d6-51ed-e7b4-b872a5fcb5bd
        set subnet 217.110.80.14 255.255.255.255
    next 
    edit "HARMFUL-IP24"
        set uuid e4094e90-d6d6-51ed-db8e-ffb99a8c2e2f
        set subnet 109.235.139.13 255.255.255.255
    next 
    edit "HARMFUL-IP25"
        set uuid e40a04ac-d6d6-51ed-b5c1-e02bee953de0
        set subnet 101.167.152.76 255.255.255.255
    next 
    edit "HARMFUL-IP26"
        set uuid e40ab1ae-d6d6-51ed-75b8-902951500f51
        set subnet 213.61.253.11 255.255.255.255
    next 
    edit "HARMFUL-IP27"
        set uuid e40b5d34-d6d6-51ed-a1f3-a1bc3393f5fe
        set subnet 213.61.253.152 255.255.255.255
    next 
    edit "HARMFUL-IP28"
        set uuid e40c0b4e-d6d6-51ed-e4b4-460bf264a01e
        set subnet 213.61.253.250 255.255.255.255
    next 
    edit "HARMFUL-IP29"
        set uuid e40cb828-d6d6-51ed-e8b0-264300168f59
        set subnet 217.110.80.14 255.255.255.255
    next 
    edit "qtn.mac_f8:5c:45:aa:08:03"
        set uuid 468117e6-f483-51ed-5f31-8508a86f239f
        set type mac
        set comment "Quarantine MAC"
        set macaddr "f8:5c:45:aa:08:03"
    next 
    edit "qtn.mac_00:00:00:00:00:00"
        set uuid 4682403a-f483-51ed-44f9-6ad5292e7a19
        set type mac
        set comment "Quarantine dummy MAC to keep the addrgrp"
    next 
    edit "glassdoor.co.in"
        set uuid d7ac2780-771c-51ee-2176-96952d4f570a
        set type fqdn
        set fqdn "*glassdoor.co.in*"
    next 
    edit "glassdoor.com"
        set uuid d7aec594-771c-51ee-29d1-8c37f8f2e9d9
        set type fqdn
        set fqdn "*glassdoor.com*"
    next 
    edit "manageengine.com"
        set uuid 0cf7a3fa-5d15-51ee-8dfe-2c0d999f91d8
        set type fqdn
        set fqdn "*manageengine.com*"
    next 
    edit "manageengine.in"
        set uuid 0cf19c08-5d15-51ee-8caf-f6aa853d6622
        set type fqdn
        set fqdn "*manageengine.in*"
    next 
    edit "zoho.in"
        set uuid 0cfd01ce-5d15-51ee-407e-bde056ab9b35
        set type fqdn
        set fqdn "*zoho.in*"
    next 
    edit "zohoassist.com"
        set uuid 0d0313ac-5d15-51ee-4d92-06eb9424af69
        set type fqdn
        set fqdn "*zohoassist.com*"
    next 
    edit "zohoassist.in"
        set uuid 0d0a10b2-5d15-51ee-a82f-2226e4ff7896
        set type fqdn
        set fqdn "*zohoassist.in*"
    next 
    edit "zohocdn.com"
        set uuid 0ceb33e0-5d15-51ee-caeb-8a1ac3ef4e96
        set type fqdn
        set fqdn "*zohocdn.com*"
    next 
    edit "securtime_device"
        set uuid 8eee60e4-d07c-51ee-ac04-06691b1fde96
        set type fqdn
        set fqdn "*device.securtime.adp.com*"
    next 
    edit "hotstar"
        set uuid 3665b388-d896-51ee-687d-961340fe1611
        set type fqdn
        set fqdn "*hotstar*"
    next 
    edit "otter.ai"
        set uuid 36693a58-d896-51ee-3747-c32afbd85e2a
        set type fqdn
        set fqdn "*otter.ai*"
    next 
    edit "telegram"
        set uuid 366bdda8-d896-51ee-ac80-92ba86b414b8
        set type fqdn
        set fqdn "*telegram*"
    next 
    edit "tiktok"
        set uuid 366e0f92-d896-51ee-9a88-d572466efe14
        set type fqdn
        set fqdn "*tiktok*"
    next 
    edit "ubembed.com"
        set uuid 7f98b51a-e808-51ee-4c93-98bdc2661be2
        set type fqdn
        set fqdn "*ubembed.com*"
    next 
    edit "co.th"
        set uuid 7f99b348-e808-51ee-64f2-6612e3840413
        set type fqdn
        set fqdn "*co.th*"
    next 
    edit "imp.onesearch.org"
        set uuid 7f9a89c6-e808-51ee-253c-bc551d9fe232
        set type fqdn
        set fqdn "*imp.onesearch.org*"
    next 
    edit "wps.com"
        set uuid 7f9b523e-e808-51ee-58c2-bc6b8d455063
        set type fqdn
        set fqdn "*wps.com*"
    next 
    edit "baidu.com"
        set uuid 7f9c1714-e808-51ee-2c94-029c56514fbc
        set type fqdn
        set fqdn "*baidu.com*"
    next 
    edit "gamepass.com"
        set uuid 7f9cdf64-e808-51ee-ada6-8307b71bebce
        set type fqdn
        set fqdn "*gamepass.com*"
    next 
    edit "anydesk.com"
        set uuid 7f9da71e-e808-51ee-2fd7-7bc6565a62d4
        set type fqdn
        set fqdn "*anydesk.com*"
    next 
    edit "spotify.com"
        set uuid 7f9e6fbe-e808-51ee-83ce-13c7ea5feee0
        set type fqdn
        set fqdn "*spotify.com*"
    next 
    edit "wpscdn.com"
        set uuid 7f9f346c-e808-51ee-3214-6937d4ad0a65
        set type fqdn
        set fqdn "*wpscdn.com*"
    next 
    edit "king.com"
        set uuid 7f9ffe74-e808-51ee-1b35-8c21b623e4f3
        set type fqdn
        set fqdn "*king.com*"
    next 
    edit "ilovepdf"
        set uuid 7fa0c3fe-e808-51ee-a469-7ca772f84aca
        set type fqdn
        set fqdn "*ilovepdf*"
    next 
    edit "WPS OFFICE"
        set uuid 30484414-e80b-51ee-7a13-9ad6f01fdd35
        set type fqdn
        set fqdn "*WPS*"
    next 
end      


config firewall addrgrp
    edit "JOD_NEW_UDR_local"
        set uuid 7b6ba274-d363-51ec-d5e9-a2c73bb89110
        set member "JOD_NEW_UDR_local_subnet_1"
        set comment "VPN: JOD_NEW_UDR (Created by VPN wizard)"
        set allow-routing enable
    next
    edit "JOD_NEW_UDR_remote"
        set uuid 7b8133a0-d363-51ec-909f-02758e95d0e9
        set member "JOD_NEW_UDR_remote_subnet_1"
        set comment "VPN: JOD_NEW_UDR (Created by VPN wizard)"
        set allow-routing enable
    next
    edit "Tikona_Server"
        set uuid 3a6a994e-db27-51ec-013f-fa44c8e1b7f6
        set member "Tikona_Capstone_Server" "Tikona_Server_1" "Tikona_Server_2" "Udaipur" "Tikona_NMS"
    next
    edit "TallyServer_new"
        set uuid b58c3310-2abb-51ed-dd1b-bb77c6923554
        set member "TallyServer1" "TallyServer2"
    next
    edit "MS_addr_quickassist"
        set uuid 5c32fc14-4211-51ed-d214-a89c5a0aa256
        set member "M1" "M10" "M11" "M12" "M13" "M14" "M15" "M16" "M17" "M18" "M19" "M2" "M3" "M4" "M5" "M6" "M7" "M8" "M9"
    next
    edit "Pharmacy trusted"
        set uuid 26524416-422e-51ed-a4a0-7b494d696593
        set member "ESHOPAID SERVER" "HIS-MAIN" "TrendMicro" "HRMAX" "JIRA" "p2p" "outlook" "ms-teams" "HDFC corporate" "DLP-SERVER" "DT-PLUS" "paramount" "Gem-employease"
    next
    edit "cash-systems"
        set uuid 25a09048-42c1-51ed-760d-ab32a1019c31
        set member "JOD-CASH02" "JOD-PHARM-02" "JOD-PHARMACY-01"
    next
    edit "Trusted"
        set uuid 5bdf5cb2-55df-51ed-ca40-b512933ae118
        set member "HIS_TRAINING" "HDFC corporate" "IIHPLMIS" "NewsLetter" "NewsLetter1" "pinopen" "TrendMicro" "Eshop_server" "P2P" "DLP-SERVER" "paramount" "HIS_TS" "manageengine.com" "manageengine.in" "zoho.in" "zohoassist.com" "zohoassist.in" "zohocdn.com" "HRMAX" "JIRA" "securtime_device"
    next 
    edit "IIHPL-IP"
        set uuid 52c0f1f2-cd4b-51ed-2cf2-8479ad6c7341
        set member "Mumbai-Primenet" "Udaipur-Airtel" "Udaipur-Ishan" "Udaipur-Tata" "Udaipur-Vodafone" "FAZ-IP" "FMG-IP"
    next 
    edit "HARMFUL-IP"
        set uuid e40d6142-d6d6-51ed-b47c-bd8b10ffe795
        set member "HARMFUL-IP1" "HARMFUL-IP10" "HARMFUL-IP11" "HARMFUL-IP12" "HARMFUL-IP13" "HARMFUL-IP14" "HARMFUL-IP15" "HARMFUL-IP16" "HARMFUL-IP17" "HARMFUL-IP18" "HARMFUL-IP19" "HARMFUL-IP2" "HARMFUL-IP20" "HARMFUL-IP21" "HARMFUL-IP22" "HARMFUL-IP23" "HARMFUL-IP24" "HARMFUL-IP25" "HARMFUL-IP26" "HARMFUL-IP27" "HARMFUL-IP28" "HARMFUL-IP29" "HARMFUL-IP3" "HARMFUL-IP4" "HARMFUL-IP5" "HARMFUL-IP6" "HARMFUL-IP7" "HARMFUL-IP8" "HARMFUL-IP9"
    next 
    edit "QuarantinedDevices"
        set uuid 4681f300-f483-51ed-38d6-2d9f5c254b07
        set member "qtn.mac_00:00:00:00:00:00" "qtn.mac_f8:5c:45:aa:08:03"
    next 
    edit "Block_in_org"
        set uuid 3670b936-d896-51ee-7981-04f9cb008a6d
        set member "hotstar" "otter.ai" "telegram" "tiktok" "anydesk.com" "co.th" "gamepass.com" "ilovepdf" "imp.onesearch.org" "king.com" "spotify.com" "ubembed.com" "WPS OFFICE" "wps.com" "wpscdn.com"
        set comment "Block_in_org"
    next 
end      

config firewall service custom
    edit "DNS"
        set category "Network Services"
        set tcp-portrange 53
        set udp-portrange 53
    next
    edit "HTTP"
        set category "Web Access"
        set tcp-portrange 80
    next
    edit "HTTPS"
        set category "Web Access"
        set tcp-portrange 443
    next
    edit "IMAP"
        set category "Email"
        set tcp-portrange 143
    next
    edit "IMAPS"
        set category "Email"
        set tcp-portrange 993
    next
    edit "LDAP"
        set category "Authentication"
        set tcp-portrange 389
    next
    edit "DCE-RPC"
        set category "Remote Access"
        set tcp-portrange 135
        set udp-portrange 135
    next
    edit "POP3"
        set category "Email"
        set tcp-portrange 110
    next
    edit "POP3S"
        set category "Email"
        set tcp-portrange 995
    next 
    edit "SAMBA"
        set category "File Access"
        set tcp-portrange 139
    next 
    edit "SMTP"
        set category "Email"
        set tcp-portrange 25
    next 
    edit "SMTPS"
        set category "Email"
        set tcp-portrange 465
    next 
    edit "KERBEROS"
        set category "Authentication"
        set tcp-portrange 88 464
        set udp-portrange 88 464
    next 
    edit "LDAP_UDP"
        set category "Authentication"
        set udp-portrange 389
    next 
    edit "SMB"
        set category "File Access"
        set tcp-portrange 445
    next 
    edit "FTP"
        set category "File Access"
        set tcp-portrange 21
    next 
    edit "FTP_GET"
        set category "File Access"
        set tcp-portrange 21
    next 
    edit "FTP_PUT"
        set category "File Access"
        set tcp-portrange 21
    next 
    edit "ALL"
        set category "General"
        set protocol IP
    next 
    edit "webproxy"
        set proxy enable
        set category "Web Proxy"
        set protocol ALL
        set tcp-portrange 0-65535:0-65535
    next 
    edit "ICMP"
        set protocol ICMP
        unset icmptype
    next 
    edit "HTTPS-IIHPL"
        set tcp-portrange 4444
    next 
    edit "ALL_TCP"
        set category "General"
        set tcp-portrange 1-65535
    next 
    edit "ALL_UDP"
        set category "General"
        set udp-portrange 1-65535
    next 
    edit "ALL_ICMP"
        set category "General"
        set protocol ICMP
        unset icmptype
    next 
    edit "ALL_ICMP6"
        set category "General"
        set protocol ICMP6
        unset icmptype
    next 
    edit "GRE"
        set protocol IP
        set protocol-number 47
    next 
    edit "AH"
        set protocol IP
        set protocol-number 51
    next 
    edit "ESP"
        set protocol IP
        set protocol-number 50
    next 
    edit "AOL"
        set visibility disable
        set tcp-portrange 5190-5194
    next 
    edit "BGP"
        set category "Network Services"
        set tcp-portrange 179
    next 
    edit "DHCP"
        set category "Network Services"
        set udp-portrange 67-68
    next 
    edit "FINGER"
        set visibility disable
        set tcp-portrange 79
    next 
    edit "GOPHER"
        set visibility disable
        set tcp-portrange 70
    next 
    edit "H323"
        set tcp-portrange 1720 1503
        set udp-portrange 1719
    next 
    edit "IKE"
        set udp-portrange 500 4500
    next 
    edit "Internet-Locator-Service"
        set visibility disable
        set tcp-portrange 389
    next 
    edit "IRC"
        set tcp-portrange 6660-6669
    next 
    edit "L2TP"
        set tcp-portrange 1701
        set udp-portrange 1701
    next 
    edit "NetMeeting"
        set visibility disable
        set tcp-portrange 1720
    next 
    edit "NFS"
        set category "File Access"
        set tcp-portrange 111 2049
        set udp-portrange 111 2049
    next 
    edit "NNTP"
        set visibility disable
        set tcp-portrange 119
    next 
    edit "NTP"
        set category "Network Services"
        set tcp-portrange 123
        set udp-portrange 123
    next 
    edit "OSPF"
        set category "Network Services"
        set protocol IP
        set protocol-number 89
    next 
    edit "PC-Anywhere"
        set category "Remote Access"
        set tcp-portrange 5631
        set udp-portrange 5632
    next 
    edit "PING"
        set category "Network Services"
        set protocol ICMP
        set icmptype 8
        unset icmpcode
    next 
    edit "TIMESTAMP"
        set protocol ICMP
        set visibility disable
        set icmptype 13
        unset icmpcode
    next 
    edit "INFO_REQUEST"
        set protocol ICMP
        set visibility disable
        set icmptype 15
        unset icmpcode
    next 
    edit "INFO_ADDRESS"
        set protocol ICMP
        set visibility disable
        set icmptype 17
        unset icmpcode
    next 
    edit "ONC-RPC"
        set category "Remote Access"
        set tcp-portrange 111
        set udp-portrange 111
    next 
    edit "PPTP"
        set tcp-portrange 1723
    next 
    edit "QUAKE"
        set visibility disable
        set udp-portrange 26000 27000 27910 27960
    next 
    edit "RAUDIO"
        set visibility disable
        set udp-portrange 7070
    next 
    edit "REXEC"
        set visibility disable
        set tcp-portrange 512
    next 
    edit "RIP"
        set category "Network Services"
        set udp-portrange 520
    next 
    edit "RLOGIN"
        set visibility disable
        set tcp-portrange 513:512-1023
    next 
    edit "RSH"
        set visibility disable
        set tcp-portrange 514:512-1023
    next 
    edit "SCCP"
        set tcp-portrange 2000
    next 
    edit "SIP"
        set tcp-portrange 5060
        set udp-portrange 5060
    next 
    edit "SIP-MSNmessenger"
        set tcp-portrange 1863
    next 
    edit "SNMP"
        set tcp-portrange 161-162
    next 
    edit "SSH"
        set tcp-portrange 22
    next 
    edit "SYSLOG"
        set category "Network Services"
        set udp-portrange 514
    next 
    edit "TALK"
        set visibility disable
        set udp-portrange 517-518
    next 
    edit "TELNET"
        set category "Remote Access"
        set tcp-portrange 23
    next 
    edit "TFTP"
        set category "File Access"
        set udp-portrange 69
    next 
    edit "MGCP"
        set visibility disable
        set udp-portrange 2427 2727
    next 
    edit "UUCP"
        set visibility disable
        set tcp-portrange 540
    next 
    edit "VDOLIVE"
        set visibility disable
        set tcp-portrange 7000-7010
    next 
    edit "WAIS"
        set visibility disable
        set tcp-portrange 210
    next 
    edit "WINFRAME"
        set visibility disable
        set tcp-portrange 1494 2598
    next 
    edit "X-WINDOWS"
        set category "Remote Access"
        set tcp-portrange 6000-6063
    next 
    edit "PING6"
        set protocol ICMP6
        set visibility disable
        set icmptype 128
        unset icmpcode
    next 
    edit "MS-SQL"
        set tcp-portrange 1433 1434
    next 
    edit "MYSQL"
        set tcp-portrange 3306
    next 
    edit "RDP"
        set category "Remote Access"
        set tcp-portrange 3389
    next 
    edit "VNC"
        set category "Remote Access"
        set tcp-portrange 5900
    next 
    edit "DHCP6"
        set category "Network Services"
        set udp-portrange 546 547
    next 
    edit "SQUID"
        set tcp-portrange 3128
    next 
    edit "SOCKS"
        set tcp-portrange 1080
        set udp-portrange 1080
    next 
    edit "WINS"
        set category "Remote Access"
        set tcp-portrange 1512
        set udp-portrange 1512
    next 
    edit "RADIUS"
        set category "Authentication"
        set udp-portrange 1812 1813
    next 
    edit "RADIUS-OLD"
        set visibility disable
        set udp-portrange 1645 1646
    next 
    edit "CVSPSERVER"
        set visibility disable
        set tcp-portrange 2401
        set udp-portrange 2401
    next 
    edit "AFS3"
        set category "File Access"
        set tcp-portrange 7000-7009
        set udp-portrange 7000-7009
    next 
    edit "TRACEROUTE"
        set category "Network Services"
        set udp-portrange 33434-33535
    next 
    edit "RTSP"
        set tcp-portrange 554 7070 8554
        set udp-portrange 554
    next 
    edit "MMS"
        set visibility disable
        set tcp-portrange 1755
        set udp-portrange 1024-5000
    next 
    edit "NONE"
        set visibility disable
        set tcp-portrange 0
    next 
edit "KOT-CASH-COUNTER"
        set type mac
        set associated-interface "lan"
        set macaddr "50:9a:4c:30:a7:04"
    next
 edit "KOT-PHARMACY"
        set type mac
        set associated-interface "lan"
        set macaddr "50:9a:4c:2f:1d:9c"
    next
end      


```
