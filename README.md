# DMCA (08/06/24)

This project was DMCA'd by some company, so all the releases, sources and everything else was wiped off, but if you still find my project useful or interesting, please leave a star <3.

___

# no-defender

A slightly more fun way to disable windows defender.

![](https://i.imgur.com/8qyJoBV.png)

## How it works

There's a WSC (Windows Security Center) service in Windows which is used by antiviruses to let Windows know that there's some other antivirus in the hood and it should disable Windows Defender.  
This WSC API is undocumented and furthermore requires people to sign an NDA with Microsoft to get its documentation.

## Limitations

Sadly, to keep this WSC stuff even after reboot, no-defender adds itself to the autorun. Thus, you would need to keep the no-defender binaries on your disk :(

## Usage
```commandline
Usage: no-defender-loader [--help] [--version] [--disable] [--firewall] [--av] [--name VAR]

Optional arguments:
  -h, --help     shows help message and exits
  -v, --version  prints version information and exits
  --disable      re-enable firewall/defender
  --firewall     disable the firewall
  --av           disable the defender
  --name         av name [default: "github.com/es3n1n/no-defender"]
```

## License
GPL-3.0
