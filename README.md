<h2 align="center">KiboCommerce, Next.JS & Amplience </h2>

<p align="center">
This is a headless ecommerce starter kit for Import hub content using Amplience cli<br>
</p>

### Features

- Import hub content from existing hub 

## Prerequisites

    Amplience account
    CLI installed on your machine: npm install -g @amplience/dc-cli

## Project Setup

1. Clone github repository
```bash
git clone https://github.com/KiboSoftware/amplience-cli.git
```
2. The CLI tool contains a lot of documentation built in to help you use each command. To get help type the following into the command line:
```bash
dc-cli --help
```

3. Each CLI tool command will require an API key and secret. This can either be specified on the command line or read from a configuration file. To set up a configuration use the configure command:
```bash
dc-cli configure --clientId <yourClientId> --clientSecret <yourSecret> --hubId <hubId>
```

## Steps - Export

1. Open cmd, go to particular folder location
2. Configure amplience 
```bash
dc-cli configure --clientId <clientId(User A)> --clientSecret <clientSecret(User A)> --hubId <hubId(User A)>
```
3. Export Content type schema
```bash
dc-cli content-type-schema export <dir>
```
4. Export Content type
```bash
dc-cli content-type export <dir>
```

## Steps - Import

1. Configure amplience 
```bash
dc-cli configure --clientId <clientId(User B)> --clientSecret <clientSecret(User B)> --hubId <hubId(User B)>
```
2. Import Content type schema
```bash
dc-cli content-type-schema import folderName --hubId <hubId(User B)>
```

3. Import Content type
```bash
dc-cli content-type import folderName --hubId <hubId(User B)>
```


## Built with

- CMS - Amplience

## Contributions

All contributions welcome!

```

```