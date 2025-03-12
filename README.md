# BestBikeApp
Repo for MicroSoft Learn Path - Develop Cloud Applications with Azure and .Net
https://learn.microsoft.com/en-us/plans/w5oizt0ep3xrg


Used PowerShell for publishing .Net 9

## Steps
1. dotnet publish -o pub
2. Compress-Archive -Path * -DestinationPath site.zip
3. Publish-AzWebApp -ResourceGroupName learn-16b4b95c-9cd3-4fe0-981f-eb3e6459082d -Name webapprw -ArchivePath .\site.zip

*Notes*
-Used a learn sandbox that only lasts for 4 hours
-Used a free learn subscription
-Make sure the Cofiguration Stack Settings are on .Net and the Major and Minor versions are .NET 9 (WebApp was created in .NET 9 and isn referenced in the csproj file)
