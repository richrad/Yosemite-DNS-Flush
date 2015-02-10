#Yosemite DNS Flush

##The Problem
You're using Yosemite and web pages stop loading. You open Console.app and see a million lines like this:

```
2/10/15 7:39:04.917 AM discoveryd[7056]: Basic DNSResolver UDNS Send(): UDP Sendto() failed to DNSNameServer 8.8.4.4 Port 53 errno 51, fd 80, ErrLogCount 27 ResolverIntf:0
```

You're _so_ mad.

##The Fix
Put this script somewhere you can access it through your PATH. I use `~/Dropbox/bin` with `export PATH=:$PATH:~/Dropbox/bin` in my `.bash_profile`.

Run `sudo flush.sh`.

Your Internet connection works again (for a while.)
