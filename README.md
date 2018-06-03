# Get-CounterStatsPlus
Gather counter values using PowerShell, and view these using the provided PowerBI template...

## Content
The main files here are the .ps1 file Get-CounterStatsPlus.ps1, and the Power BI template Get-CounterStatsPlus-PBI.pbit.

## How to use these
### Collecting counters with the provided Powershell script
First use Get-CounterStatPlus.ps1 to collect counters either from the local machine (launch it without any options):

```
.\Get-CounterStatsPlus.ps1
```

or counters from multiple machines /You need Admin permissions on these machines to collect counters remotely - typically a Domain Admin account has the right to do these for machines of the domain he's admin from - the synthax would be :

```
.\Get-CounterStatsPlus.ps1 -ServersTXTfile C:\temp\Myservers.txt -NumberOfSamples 60 -OutputFile c:\ExportRequestISsue.csv
```

To get more help topics, on Powershell use the Powershell Get-Help such as :
```
Get-Help .\Get-CounterStatsPlus.ps1 -Full
```
For full help
```
Get-Help .\Get-CounterStatsPlus.ps1 -Details
```
For detailed help
```
Get-Help .\Get-CounterStatsPlus.ps1 -Examples
```
For examples only.
### Visualizing your collected counters with the provided PowerBI Template
This is simple, after having installed PowerBI, just double-click on the Get-CounterStatsPlus-PBI.pbit file provided, put in the full path to the .CSV file that you collected with the above described PowerShell script, and see the magic !

![test image size|883x282,20%](//Screenshots/PBI-ChooseCSVtoanalyze.png "height=10px")

![test](https://github.com/favicon.ico:height="24px" width="48px")

![very good|200%](https://github.com/favicon.ico)

