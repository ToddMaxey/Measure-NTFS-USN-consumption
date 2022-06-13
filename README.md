# Measure-NTFS-USN-consumption
Powershell script to query the NTFS USN journal to determine if you have a high USN consumption rate.

Measure-UsnConsumption

Useage:

Measure-UsnConsumption [-DurationInSeconds][-UsnConsumptionThreshold][-DriveLetter][-DriveLetter]


Switches:

-DurationInSeconds    Duration between the sample of NextUSN. Default is 60 seconds

-UsnConsumptionThreshold    The threshold that a event log error will be generated based on the difference between the new NextUSN samples. Default is 1,000,000

-DriveLetter    The volume to run the test agains. Default is the volume of the system drive.

-LogEvent    Log results in System event log. Boolean. Default is $True

