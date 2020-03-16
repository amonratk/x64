# How to fix pull/push with schannel

## When do you pull/push

`fatal: unable to access 'https://github.com/prawee/symfony5.git/': schannel: next InitializeSecurityContext failed: Unknown error (0x8
0092013) - The revocation function was unable to check revocation because the revocation server was offline.`

## Fixed

```bash
$ git config --global http.sslBackend openssl
$ git config --global http.sslVerify true
```

## Testing

```bash
$ git pull
Already up to date.
```
