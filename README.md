# DuckDNS snap

[![Snap Status](https://build.snapcraft.io/badge/kyrofa/duckdns.svg)](https://build.snapcraft.io/user/kyrofa/duckdns)

This simple snap updates the configured DuckDNS domain names every five
minutes. Configure it by providing your token:

    $ snap set duckdns-kyrofa token=<secret>

And configure your domain name list (comma-separated, no spaces):

    $ snap set duckdns-kyrofa domains=domain1.com,domain2.com

That's it. The daemon runs every five minutes. Check the journal for output,
including any problems:

    $ journalctl -u snap.duckdns-kyrofa.duckdns.service
