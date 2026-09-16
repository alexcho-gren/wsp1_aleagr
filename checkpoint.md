UTDATA FRÅN SWITCH-1:
Switch-1#show interfaces trunk
Port        Mode         Encapsulation  Status        Native vlan
Gig0/1      on           802.1q         trunking      999

Port        Vlans allowed on trunk
Gig0/1      10,20,30

Port        Vlans allowed and active in management domain
Gig0/1      10,20,30

Port        Vlans in spanning tree forwarding state and not pruned
Gig0/1      10,20,30


Switch-1#show vlan brief

VLAN Name                             Status    Ports
---- -------------------------------- --------- -------------------------------
1    default                          active    Fa0/4, Fa0/5, Fa0/6, Fa0/7
                                                Fa0/8, Fa0/9, Fa0/10, Fa0/11
                                                Fa0/12, Fa0/13, Fa0/14, Fa0/15
                                                Fa0/16, Fa0/17, Fa0/18, Fa0/19
                                                Fa0/20, Fa0/21, Fa0/22, Fa0/23
                                                Fa0/24, Gig0/2
10   KONTOR                           active    Fa0/1
20   EKONOMI                          active    Fa0/2
30   GAST                             active    Fa0/3
99   DRIFT                            active    
999  NATIVE                           active    
1002 fddi-default                     active    
1003 token-ring-default               active    
1004 fddinet-default                  active    
1005 trnet-default                    active    




UTDATA FRÅN SWITCH-2:
Switch-2#show interfaces trunk
Port        Mode         Encapsulation  Status        Native vlan
Gig0/1      on           802.1q         trunking      999

Port        Vlans allowed on trunk
Gig0/1      10,20,30

Port        Vlans allowed and active in management domain
Gig0/1      10,20,30

Port        Vlans in spanning tree forwarding state and not pruned
Gig0/1      10,20,30


Switch-2#show vlan brief

VLAN Name                             Status    Ports
---- -------------------------------- --------- -------------------------------
1    default                          active    Fa0/4, Fa0/5, Fa0/6, Fa0/7
                                                Fa0/8, Fa0/9, Fa0/10, Fa0/11
                                                Fa0/12, Fa0/13, Fa0/14, Fa0/15
                                                Fa0/16, Fa0/17, Fa0/18, Fa0/19
                                                Fa0/20, Fa0/21, Fa0/22, Fa0/23
                                                Fa0/24, Gig0/2
10   KONTOR                           active    Fa0/1
20   EKONOMI                          active    Fa0/2
30   GAST                             active    Fa0/3
999  NATIVE                           active    
1002 fddi-default                     active    
1003 token-ring-default               active    
1004 fddinet-default                  active    
1005 trnet-default                    active    



SKÄRMDUMPAR:

PC-1 PING: 

<img width="1748" height="1109" alt="Image" src="https://github.com/user-attachments/assets/285de205-ecf7-4075-930e-16e6d617ec29" />

PC-2 PING:

<img width="1728" height="1134" alt="Image" src="https://github.com/user-attachments/assets/1b455206-16b3-4b55-8ba5-167bd52d4128" />

Switch-1: Utdata från show interfaces trunk och show vlan brief:

<img width="1719" height="1013" alt="Image" src="https://github.com/user-attachments/assets/b54480d9-738e-4b2e-a419-4b26b128110c" />

<img width="1668" height="1036" alt="Image" src="https://github.com/user-attachments/assets/0ed59a24-f88f-4264-baa0-34121a54a56d" />


Switch-2: Utdata från show interfaces trunk och show vlan brief:

<img width="1606" height="951" alt="Image" src="https://github.com/user-attachments/assets/614ed1bc-86cd-452e-8704-16455d4d62f7" />

<img width="1714" height="1009" alt="Image" src="https://github.com/user-attachments/assets/c90a9292-3064-4133-bde7-3b056db37cbe" />
