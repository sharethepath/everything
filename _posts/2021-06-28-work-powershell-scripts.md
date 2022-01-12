---
title: "Post: Scripts For Work"
categories: 
  - Tech
  - Blog
tags:
  - PowerShell
  - Joy To Work
  - Skills 
---
For marketing purposes or just to have a better picture, here is a nice tool: 

### makes a word cloud from copied text
On a Windows machine press Win+X, then press 'I' that will launch PowerShell (on a Mac you might install PowerShell first). 
Afterwards install a module. 
```PowerShell
Install-Module PSWordCloud
```
Press [Y]es along the way to allow the install. 
When it's done, you will be able to copy the text and run the command below to generate your word cloud. 
```PowerShell
Get-Clipboard | New-WordCloud -Path .\wordcloud.svg -Typeface georgia -ImageSize 720p -AllowRotation none
```

More info about the details and setting of your wordcloud can be found with PSWordCloud module, that is made by Joel Sallow, here is his [blog post about it](https://vexx32.github.io/2018/12/06/Scripting-Fun-Word-Cloud-Generator/)

### This search is of handy when you have plenty of files on a computer and need to filter your search by extensions. 
### Advanced search with PowerShell
source: [devblogs.microsoft.com](https://devblogs.microsoft.com/scripting/use-windows-powershell-to-search-for-files/)

Get-Childitem –Path C:\ -Recurse
Get-Childitem –Path C:\ -Include *HSG* -Exclude *.JPG,*.MP3,*.TMP -File -Recurse -ErrorAction SilentlyContinue 

#### Updated: 2021-06