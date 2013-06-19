# Vertkl - Bootstrap

`vertkl.org` is an aggregation of information. A node on the internet which collects information about climbing routes.

Climbing routes, or `climbs` as we call them, come in many shapes and sizes. There are bouldering problems, trad climbs, sport climbs, multi-pitch climbs, ice climbs, mixed climbs.

`vertkl.org` comes in two parts. For humans, there is a website which you can access at [http://vertkl.org] where you can register, search climbs and also add them to your logbook or tick list.

For machines, you can also access a machine readable version of the data at [http://api.vertkl.org]. This means that all of the information in `vertkl` is available to anyone who wants to build a client.

# Developer machine setup

You will need a few things.

## nginx

   brew install nginx



To have launchd start nginx at login: 

   ln -sfv /usr/local/opt/nginx/*.plist ~/Library/LaunchAgents 

Then to load nginx now: 

     launchctl load ~/Library/LaunchAgents/homebrew.mxcl.nginx.plist