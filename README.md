# Linux Disk Usage Scripts

Two simple `Linux` disk usage monitoring scripts that sends an email notification if certain conditions are met. Two scripts utilise both MB Block usage and
default disk capacity usage for a particular a `POSIX` partition. If both are greater than thresholds, then trigger the email alert through the system.

## Example

A sample of output for `df` looks like:

```
	 example% df
	 Filesystem   kbytes  used  avail  capacity  Mounted on
	 ojd2:/	        7445  4714   1986    70%       /
	 ojd2:/usr     42277  35291  2758    93%       /usr
```
Both scripts utilise the `df -h` and the `df -M` commands which both display both disk usage statistics and MB Block disk usage amount. If either two is
greater than or equal to thresholds, some simple methods send email notifications.