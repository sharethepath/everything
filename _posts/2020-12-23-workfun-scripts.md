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

### makes a word cloud from copied text
On a Windows machine press Win+X, then press 'I' that will launch PowerShell. 
Afterwards install a module. 
```PowerShell
Install-Module PSWordCloud
```
When it's done, you will be able to copy the text and run the command below to generate your word cloud. 
```PowerShell
Get-Clipboard | New-WordCloud -Path .\wordcloud.svg -Typeface georgia -ImageSize 720p -AllowRotation none
```

More info about the details and setting of your wordcloud can be found with PSWordCloud module, that is made by Joel Sallow, here is his [blog post about it](https://vexx32.github.io/2018/12/06/Scripting-Fun-Word-Cloud-Generator/)

### Advanced search with PowerShell
source: [devblogs.microsoft.com](https://devblogs.microsoft.com/scripting/use-windows-powershell-to-search-for-files/)

Get-Childitem –Path C:\ -Recurse
Get-Childitem –Path C:\ -Include *HSG* -Exclude *.JPG,*.MP3,*.TMP -File -Recurse -ErrorAction SilentlyContinue 
