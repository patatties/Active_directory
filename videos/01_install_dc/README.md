# 01 installing the domain controller

1. use 'sconfig' to:
    change hostname
    change ip address to static
    change DNS setting

2. Install Windows AD feature:
    PS> install-windowsfeature AD-Domain-Services -includemanagementtools
