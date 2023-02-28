# 00 preparing the VMs

1. Workstation Windows 11
    - open CMD prompt in Setup
    - regedit
    - add regkeys:
        [HKEY_LOCAL_MACHINE\SYSTEM\Setup\LabConfig]
            "BypassTPMCheck"=dword:00000001
            "BypassSecureBootCheck"=dword:00000001
            "BypassRAMCheck"=dword:00000001


2. Server Windows XX



3. Snapshot and template
    - Shutdown the machine in desired state
    - Create snapshot Fresh Install
    - In VM Settigns, select options tab, Select advanced, check: Enable Template Mode