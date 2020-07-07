# dotnet-docker

A simple wrapper to run the .NET Core SDK and Runtime from a Docker container.

Uses the official [Microsoft .NET Core SDK image](https://hub.docker.com/_/microsoft-dotnet-core-sdk/) using the `3.1` tag (Debian 10)

Based on the Docker Compose [Run docker-compose in a container](https://github.com/docker/compose/blob/1.25.4/script/run/run.sh) script.

## Installation

```bash
sudo curl -L --fail https://github.com/bshaw/dotnet-docker/blob/v1.0.1/run.sh -o /usr/local/bin/dotnet
sudo chmod +x /usr/local/bin/dotnet
```

## Usage

Use the dotnet command as you would if it were installed locally.

```bash
❯ dotnet --info
.NET Core SDK (reflecting any global.json):
 Version:   3.1.301
 Commit:    7feb845744

Runtime Environment:
 OS Name:     debian
 OS Version:  10
 OS Platform: Linux
 RID:         debian.10-x64
 Base Path:   /usr/share/dotnet/sdk/3.1.301/

Host (useful for support):
  Version: 3.1.5
  Commit:  65cd789777

.NET Core SDKs installed:
  3.1.301 [/usr/share/dotnet/sdk]

.NET Core runtimes installed:
  Microsoft.AspNetCore.App 3.1.5 [/usr/share/dotnet/shared/Microsoft.AspNetCore.App]
  Microsoft.NETCore.App 3.1.5 [/usr/share/dotnet/shared/Microsoft.NETCore.App]

To install additional .NET Core runtimes or SDKs:
  https://aka.ms/dotnet-download
```
