# Custom npm init

**Inspiration**
---
I'm a programmer. That inherently means I hate repeating myself. I went on a research mission to see how I could automate my npm init and customise it to make it a smoother and easier experience that doesn't rely on shell scripting.


I discovered the following websites, but there wasn't a whole lot of documentation of examples that I could find so, through trial and error I came up with the `config.js` above. I wanted to find a way to run `npm install` within the config file but I couldn't quite get it this time around.
[NPM package](https://www.npmjs.com/package/init-module?activeTab=readme/)

[Inspirational Repo](https://github.com/npm/init-package-json)

## Steps to install:
  First run `npm config ls -l` to see all of your settings. it should look something like the [example file above](./exampleConfig.txt)
  
  **NOTE:** _Anywhere you see a semi-colon`";"`it just means a comment so don't delete everthing!_ [Look here for an example](./commented-out-example.txt)

  You'll notice that you have multiple config files, and just like your `.git` config files they follow a hierarchy of importance. Closest to the folder is the active one. To make things easier for me, I went ahead and changed all of them to match so I would have a consistent npm experience.

  **Directory List**
  Your's may be different but they should be in the same general location.
  
|Title|Path|
|---|---|
|User|C:\Users\mk\.npmrc|
|Global|C:\Users\mk\AppData\Roaming\npm\etc\npmrc|
|Builtin undefined| C:\Users\mk\AppData\Roaming\npm|

I commented every setting out then picked the ones I like best. From there it was just a matter o