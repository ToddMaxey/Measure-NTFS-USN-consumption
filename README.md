# Measure NTFS USN consumption
PowerShell script to query the NTFS USN journal to determine if you have a high USN consumption rate or if the USN journal has a new identifier. Script Utility - Identify USN journal consumption issue causing USN Journal wrap. Identify changes to the USN Journal where the journal size or identifier is changed. Components or processes affected: Distributed File System Replication, File System Index, File System forensics.

PowerShell Command: Measure-UsnConsumption

Usage:

Measure-UsnConsumption [-DurationInSeconds][-UsnConsumptionThreshold][-DriveLetter][-DriveLetter]

Switches:

-DurationInSeconds
 Duration between the sample of NextUSN. Default is 60 seconds

-UsnConsumptionThreshold
 The threshold that a event log error will be generated based on the difference between the new NextUSN samples. Default is 1,000,000

-DriveLetter
 The volume to run the test agains. Default is the volume of the system drive.

-LogEvent
 Log results in System event log. Boolean. Default is $True
