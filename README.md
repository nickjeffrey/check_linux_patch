# check_linux_patch
nagios check to show days since last Linux OS patching, and number of available updates

# Requirements
perl, access to upstream repos to query available updates


# Sample Output

```
Linux patch level OK - CentOS9 was last patched 2 days ago on 2025-01-15. Available updates:0 | linux_version=CentOS9;;;; days_since_patch=2;;;; available_updates=0;;;
````

````
Linux patch level OK - Ubuntu22.04LTS was last patched 0 days ago on --. Available updates:283 updates:115 security_updates:168 | linux_version=Ubuntu22.04LTS;;;; days_since_patch=0;;;; available_updates=283;;;;
````

````
Linux patch level WARN - RHEL subscription state is unknown, cannot query upstream repos for available patches.  | linux_version=RHEL8.5;;;; days_since_patch=1;;;; available_updates=0;;;;
```

```
Linux patch level WARN - RHEL9.1 was lated patched 181 days ago on 2024-06-14.   Available updates:1452 bugfix:956 enhancement:35 Security_Low:29 Security_Moderate:270 Security_Important:160 Security_Critical:0 | linux_version=RHEL9.1;;;; days_since_patch=181;;;; available_updates=1452;;;;
```
