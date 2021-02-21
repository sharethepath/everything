---
title: "Post: Blogging and Jekyll"
tags:
  - PowerShell
  - Git
  - Jekyll blogging
  - Microsoft 
---
<meta name="msvalidate.01" content="7A96D455B03667537A649E9E535AC3CF" />

Git and GitHub, PowerShell, VS Code. 
Adding to this mix Jekyll with Minimal Mistakes theme. 

## sources:
1. [Start using Git for PowerShell scripts](https://4bes.nl/2019/06/02/step-by-step-start-using-git-for-powershell/) The path travelled, and support on this way. 
  Prerequisites on Windows: 
  - Ruby (option with Ruby Installer or with WSL), Ruby gems
  - Git, GitHub account, 
  - VS code and PowerShell. 
2. Then followed the guide from Holistic Security: 
[holistic security](https://holisticsecurity.io/2020/03/30/github-pages-and-jekyll-on-windows-10)
  `bundle exec jekyll serve `
3. [Blogging with Jekyll using Minimal Mistakes Theme](https://purple.telstra.com.au/blog/opensource-blogging-with-jekyll-github-vscode-part-2)
Got an error doing $bundle exec jekyll serve while executing Remote Theme (Minimal-Mistakes): Could not find gem 'github-pages x64-mingw32' in any of the gem sources listed in your Gemfile.
Run `bundle install` to install missing gems.

~~~
other refereces: 
Sean Killeen - building Jekyll blog
~~~

## Adding Bing Analytics 

## Setting comments and Analytics: 
[Katerina's website](https://www.cross-validated.com/Personal-website-with-Minimal-Mistakes-Jekyll-Theme-HOWTO-Part-IV/)

Adding trackers to "_config.yml" 
> Measurement ID: (same as tracking_id, by Google)
> can add google tracking_id and set anonymize_ip to true

analytics:
  provider: "google"
  google:
    tracking_id: "" 
    anonymize_ip: true

bing_site_verification: "" (lenghty string comes here)


