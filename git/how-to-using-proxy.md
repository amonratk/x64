# How to using proxy

## Problem

`fatal: unable to access 'https://github.com/prawee/x64.git/': Failed to connect to github.com port 443: Timed out`

## Solved

### Checking current configure

```bash
> git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=schannel
core.autocrlf=true
core.fscache=true
core.symlinks=false
credential.helper=manager
```

### Using proxy

```bash
git config --global http.proxy http://domain.local\v{user}:{pass}@{proxy_server}:{port}
```

### Unset proxy

```bash
git config --global --unset http.proxy
```
