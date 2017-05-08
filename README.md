**Documentation**
PSScriptAnalyzer rules suggesting optimizations for loop statements 'For'.

[Optimization rules](https://github.com/LaurentDardenne/OptimizationRules/tree/master/RuleDocumentation)

**PowerShell 5 Installation, (development version)**

From PowerShell run:
```Powershell
$PSGalleryPublishUri = 'https://www.myget.org/F/ottomatt/api/v2/package'
$PSGallerySourceUri = 'https://www.myget.org/F/ottomatt/api/v2'

Register-PSRepository -Name OttoMatt -SourceLocation $PSGallerySourceUri -PublishLocation $PSGalleryPublishUri #-InstallationPolicy Trusted

Install-Module OptimizationRules -Repository OttoMatt -Verbose -Force
```


