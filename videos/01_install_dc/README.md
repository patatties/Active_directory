# 01 installing the domain controller

1. use 'sconfig' to:
    - change hostname
    - change ip address to static

2. Install Windows AD feature:
    - install-windowsfeature AD-Domain-Services -includemanagementtools
    - Import-Module ADDSDeployment
    - Install-ADDSForest
Reboot
    - Set DNS Server
        - get-netadapter
        - Set-DNSClientServerAddress -interfaceindex <no> -ServerAddresses 192.168.2.155

3. Adding computers to domain:
- get-netadapter
- Set-DNSClientServerAddress -interfaceindex <no> -ServerAddresses 192.168.2.155
- Add-Computer -DomainName tt.local -Credential tt\Administrator -Force -Restart