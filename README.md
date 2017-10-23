# <img src="https://github.com/iqp-samples/iqp-samples-ws/raw/master/logo.png" alt="iQuipsys Logo" style="max-width:30%"> <br/> Workspace for iQuipsys Positron Samples

This is a workspace for [IQuipsys Positron](http://www.iquipsys.com) samples.
It enables build, test, and release across the following projects:

- **iqp-samples-integration-excel** - Excel integration sample
- **iqp-samples-integration-ps** - Powershell integration sample
- **iqp-samples-integration-sqlserver** - SQL Server integration sample

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/iqp-samples/iqp-samples-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The sample projects are created and maintained by:
- **Dmitry Krainiy**
- **Sergey Seroukhov**
- **Anatoly Makarychev**
