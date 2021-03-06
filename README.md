---
---

# Dashboard

[![Build Status](https://travis-ci.org/jwronline/dashboard.svg?branch=gh-pages)](https://travis-ci.org/jwronline/dashboard)

This is a dashboard to use with a space shuttle flight following [shuttle-command](http://gh.jwronline.be/shuttle-command/) and [jwr-shuttle](https://github.com/jwronline/jwr-shuttle) for scripts.

Inspired by NASA's [MCC](https://en.wikipedia.org/wiki/Christopher_C._Kraft_Jr._Mission_Control_Center)

![screenshot](src/img/screenshot.png)

## Usage

### Setup

There are several ways to running this dashboard

#### Static (1 display)

Go to the ["releases"](https://github.com/jwronline/dashboard/releases/) tab and download the newest version of `Shuttle-platform.zip`. You can unzip that and open the program.

- updated ISS data if an internet connection present
- a program
- 1 display
- completely offline
- easy

#### Online (multiple displays)

Go to [gh.jwronline.be/dashboard/](http://gh.jwronline.be/dashboard/) on every computer you want to see it.

- needs to have network
- works in the browser
- up to date ISS data
- not automatically synchronised (you need to push synchronously)
- easiest

#### Offline but networked (multiple displays)

> This mode needs to be made

Clone the repository from github like this:

```sh
$ git clone https://github.com/jwronline/dashboard.git
$ cd dashboard
```

Once inside you have to make sure you've got internet connection (for the setup, later can be used offline) and have installed [nodejs](https://nodejs.org/en/download/). Then you run:

```sh
$ npm install
$ gulp serve
```

This will setup a local server that will mirror all keypresses etc. to the other devices you have running. Make sure that all the devices are on the same network and then open in the browsers the address that is returned by `gulp`. This is `http://your-ip-address:3000`.

> Note: this hasn't been made yet.

- synchronised displays
- updated ISS data if an internet connection present
- best
- technically harder

### controls

* advance a step
    * spacebar
    * enter
    * down arrow
    * righ arrow
* go back a step
    * backspace
    * up arrow
    * left arrow
* toggle holding state (MET)
    * p
    * h
* toggle help
    * ?
* show remote
    * r

### Other resources

The script that has to be used while running this dashboard is available to view at [gh.jwronline.be/scripts/](http://gh.jwronline.be/scripts/) and on [github](https://github.com/jwronline/scripts). The program that's used currently for each computer individually is also on [github](https://github.com/jwronline/shuttle-commmand). An overview of the whole project is available at [gh.jwronline.be/jwr-shuttle](http://gh.jwronline.be/jwr-shuttle).

## Contributing

Right now this is a shell of what it could become, it can use real data, more variable data and more configuring. It should also in long term be connected to what the players see and enter on their consoles.

## License

Icon is based on [Space Shuttle by Giuditta Valentina Gentile from the Noun Project](https://thenounproject.com/term/space-shuttle/302031/).

[![Creative Commons Licence](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/4.0/)

This is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/). No warranty whatsoever.

Made by [Haroen Viaene](https://haroen.me) for [JWR v.z.w.](http://jwronline.be).
