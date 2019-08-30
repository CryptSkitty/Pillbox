# Pillbox
A robust firewall designed for use by penetration testing machines, specifically Kali.

Installation:
  The script is manually evocable, lending itself well to direct calling via ifupdown, but also supports systemctl calls if placed in init.d. How & where you install it is up to you. While disabling NetworkManager is not required, it is recommended, as certain functions in pillbox assume low-level control of devices that NM may take issue with.

Using Pillbox:
  Pillbox works like a traditional iptables based firewall, with a few notable exceptions. Pillbox supports the usage of iptables-save, but does not automatically load saved states. Instead, pillbox loads it's 'base state' as configured in the script, and when prodded, will load other states. Certain functions of pillbox require a bit of host configuration in the way of slight modifications to Nmap. Sudo configuration is encouraged.

Contributing:
  If you wish to contribute, by all means do, just reach out.
