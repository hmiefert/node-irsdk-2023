# node-irsdk-2023

Unofficial [iRacing](http://www.iracing.com/) SDK implementation for NodeJS.

## DISCLAIMER
First of all I'm a self-taught coder and wouldn't call myself a developer as I have no educational background.

As I had various errors with the original repo [node-irsdk](https://github.com/apihlaja/node-irsdk) By Antti Pihlaja
and also several forks, I've tried to puzzle the barebones pieces together to get this version running, starting with
[node-irsdk-2021](https://github.com/mcalapurge/node-irsdk) By Nekaiko.

So, this version works as of 30/12/2022 and NodeJS v18.12.1 LTS, with no prebuild and only the necessary dependencies to get it up and running, but at least no vulnerabilities, so that's good I guess.
Also there is none of the previous testing framework.

## prerequesites
For compiling this package you need `node-gyp@^9.0.0`.
```
npm install -g node-gyp
```
You also need a current version of `Python3` and `Microsoft Visual Studio Build Tools` installed.
More information regarding the topic can be found [here](https://github.com/nodejs/node-gyp#on-windows).

## installing the package
```
npm install --save https://github.com/hmiefert/node-irsdk-2023
```

## using with electron
When using this package with electron, you might run into an error stating that the installed package was compiled against a different version of NodeJS, therefore the NODE_MODULE versions differ and you're expected to recompile the package.
To achieve this you need a package called electron-rebuild and run the rebuild command manually:
```
npm install --save-dev electron-rebuild
.\node_modules\.bin\electron-rebuild.cmd
```

## further information
* [documentation](https://apihlaja.github.io/node-irsdk)
* [original forum thread](http://members.iracing.com/jforum/posts/list/3329583.page)
* [new forum thread](https://forums.iracing.com/discussion/34241/does-node-irsdk-still-work)

Other iRSDK implementations:

* [Official C/C++ SDK](http://members.iracing.com/jforum/posts/list/1470675.page)
* [iRacingSdkWrapper (C#)](https://github.com/NickThissen/iRacingSdkWrapper)
* [pyirsdk (python3)](https://github.com/kutu/pyirsdk/)
* [iRacingSDK.Net](https://github.com/vipoo/iRacingSDK.Net)

