freebsd-pf-script
=================

experimental script(s) for setting up FreeBSD's pf firewall

# Usage

Setup /etc/pf/pf.conf

```
gdf
```

Check for bad login attempts

```
pf-sshinvaliduserip -a
```

Add invalid login attempts to blacklist by ip

```
pf-sshinvaliduserip block
```

View your sshban list

```
pf-table show sshban
```

Remove an item from your sshban list

```
pf-table remove sshban 8.8.8.8
```
