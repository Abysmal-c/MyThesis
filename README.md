Please check following files and codes... 
Node:
Mac_802_15_4_Node -> app_mac_802_15_4_process.c -> APP_MAC_mcpsDataIndCb (This is Where incoming message is analyzed and the related BE_min value is fetched)
Mac_802_15_4_NodeA -> app_mac_802_15_4.c -> APPE_Button2Action (This is where Data is sent, BE_min value is changed according to the incoming data and LED indication is provided in the way that one blink for BE_min=0, three blink for BE_min=3)
Coordinator:
Mac_802_15_4_Coordinator -> app_mac_802_15_4.c -> APPE_Button2Action (BE_min= 0 is sent) and APPE_Button3Action (BE_min=3 is sent)
