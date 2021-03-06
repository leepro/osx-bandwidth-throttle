# OSx Bandwidth Throttler (this will work for any *nix)

## Basic Usage

- Download throttle.sh.
- Make the file executable with `chmod +x throttle.sh`
- Run it as the admin with `sudo ./throttle.sh 45`
- Turn everything off by running `sudo ./throttle.sh stop`

## Values

- Numerical values will adjust to that speed in Kbytes/s e.g. `sudo ./throttle.sh 54`
- Typing stop will reset back to what it should be e.g. `sudo ./throttle.sh stop`
- Typing some predefined constants will result in some throttling e.g. `sudo ./throttle.sh 3g`

## Constants taken from here (http://www.which.co.uk/technology/phones/guides/mobile-broadband/mobile-broadband-speed-and-usage-limits/)

- gprs - 30
- edge - 200
- 3g - 14000
- 4g - 3000000

## Help!

If you manage to throttle your speed but can't get it to go back to normal you should run this command: `sudo ipfw delete 1`

## Thanks

The initial code for building this was inspired by this article by Ben Lakey - http://benlakey.com/2012/10/14/throttle-bandwidth-on-mac-os-x/