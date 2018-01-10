## damdo/sscratch

:key: **s**(ecure)**scratch** - the docker SCRATCH image with SSL ca-certificates

### FEATURES:
 - `FROM scratch` + `ca-certificates.crt` (for SSL connections)
 - Optimized for Minimal Possible Size ~**236kB**
 - Easy to remember


### USAGE:
In your Dockerfile
```python
FROM damdo/sscratch

# do your awesome things here ...

```

### MANUAL BUILD:
```sh
docker build -f Dockerfile-build -t yourimagename .
```

### OTHER:
The certs are automatically downloaded from: https://curl.haxx.se/docs/caextract.html <br>
They are *constantly* updated and comes from the Mozilla CA certificate store: https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/
