# How to configure global settings

## Name and Email

```bash
> git config --global user.name "Prawee Wongsa"
> git config --global user.email "prawee.wongsa@allianz.com"
```

## Checking configure list

```bash
> git config --list
```

Result
```bash
...
user.name=Prawee Wongsa
user.email=prawee.wongsa@allianz.com
...
```

## Fix Identity

```bash
> git commit --amend --reset-author
```
