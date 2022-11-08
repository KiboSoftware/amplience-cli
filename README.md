<h2 align="center">KiboCommerce & Amplience </h2>

<p align="center">
This is a repo containing Amplience Content Types and Schemas used in KiboCommerce demo starter kits<br>
</p>

### Features

- Import hub content from existing hub 

## Prerequisites

1.  Amplience account
2.  Amplience ClientID, ClientSecret, and HubID

## Project Setup

1. CLI installed on your machine: npm install -g @amplience/dc-cli
2. Clone github repository
```bash
git clone https://github.com/KiboSoftware/amplience-demo-data.git
```
3. The CLI tool contains a lot of documentation built in to help you use each command. To get help type the following into the command line:
```bash
dc-cli --help
```

4. Each CLI tool command will require an API key and secret. This can either be specified on the command line or read from a configuration file. To set up a configuration use the configure command:
```bash
dc-cli configure --clientId <yourClientId> --clientSecret <yourSecret> --hubId <hubId>
```

## Steps - Import

1. Configure amplience 
```bash
dc-cli configure --clientId <importClientId> --clientSecret <importClientSecret> --hubId <importHubId>
```
2. Import Content type schema
```bash
dc-cli content-type-schema import folderName --hubId <importHubId>
```

3. Import Content type
```bash
dc-cli content-type import folderName --hubId <importHubId>
```

## Steps - Export

1. Open cmd, go to particular folder location
2. Configure amplience 
```bash
dc-cli configure --clientId <exportClientId> --clientSecret <exportClientSecret> --hubId <exportHubId>
```
3. Export Content type schema
```bash
dc-cli content-type-schema export <dir>
```
4. Export Content type
```bash
dc-cli content-type export <dir>
```


## Built with

- CMS - Amplience

## Contributions

All contributions welcome!

```

```