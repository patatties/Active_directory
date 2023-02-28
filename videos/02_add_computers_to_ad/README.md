# adding systems to the domain

- get-netadapter
- Set-DNSClientServerAddress -interfaceindex <no> -ServerAddresses 192.168.2.155
- Add-Computer -DomainName tt.local -Credential tt\Administrator -Force -Restart