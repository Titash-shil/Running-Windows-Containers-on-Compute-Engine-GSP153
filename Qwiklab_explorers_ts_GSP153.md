# Running Windows Containers on Compute Engine || [GSP153](https://www.cloudskillsboost.google/focuses/3348?parent=catalog) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝
### Run the following Commands in Command Prompt

```
docker images
mkdir my-windows-app
cd my-windows-app
mkdir content
call > content\index.html
notepad content\index.html
```
```
<html>
  <head>
    <title>Windows containers</title>
  </head>
  <body>
    <p>Windows containers are cool!</p>
  </body>
</html>
```
```
call > Dockerfile
notepad Dockerfile
```
```
FROM mcr.microsoft.com/windows/servercore/iis:windowsservercore-ltsc2019

RUN powershell -NoProfile -Command Remove-Item -Recurse C:\inetpub\wwwroot\*

WORKDIR /inetpub/wwwroot

COPY content/ .
```
```
docker build -t gcr.io/dotnet-atamel/iis-site-windows .
docker images
```

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 
