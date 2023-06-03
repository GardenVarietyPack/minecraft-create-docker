# Minecraft Server 

docker-compose for the Forge modded server with the Create mod installed.

Using the following Docker images: 

| Docker Image                   | Dockerhub                                                               | Github                                                                          |
|--------------------------------|-------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| itzg/minecraft-server:latest   | [itzg/minecraft-server](https://hub.docker.com/r/itzg/minecraft-server) | [itzg/docker-minecraft-server](https://github.com/itzg/docker-minecraft-server) |

( See docker-compose.yml )

## Quickstart

```
docker-compose up
```

Ensure `/server` dir has proper permissions:

On Windows: `takeown /F server /A /R` 
On Linux/OSX: `chown -R server`

**NOTE**: By providing EULA=TRUE you agree to the EULA at https://account.mojang.com/documents/minecraft_eula.

## Environment Variables
- EULA (Required)
  - Default: none

## Docs / Guides

See [client-setup-guide.md](docs/client-setup-guide.md) to setup your minecraft client.

## Mods List

| Mod Name                                                                   | Mod File Path                            |
|----------------------------------------------------------------------------|------------------------------------------|
| [Create](https://www.curseforge.com/minecraft/mc-mods/create)              | `mods\create-1.19.2-0.5.1.b.jar`         |
| [JEI](https://www.curseforge.com/minecraft/mc-mods/jei)                    | `mods\jei-1.19.2-forge-11.6.0.1015.jar`  |
| [Journey Map](https://www.curseforge.com/minecraft/mc-mods/journeymap)     | `mods\journeymap-1.19.2-5.9.7-forge.jar` |
