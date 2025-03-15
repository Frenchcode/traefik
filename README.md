# Traefik

This is a traefik setup template you to setup a a reverse-proxy for all your docker containers 

## Key Concept

Traefik is based on the concept of EntryPoints, Routers, Middlewares and Services.

- **EntryPoints**:  are the network entry points into Traefik. They define the port which will receive the packets, and whether to listen for TCP or UDP.
- **Routers**: is in charge of connecting incoming requests to the services that can handle them.
- **Middlewares**: Attached to the routers, middlewares can modify the requests or responses before they are sent to your service
- **Services**: are responsible for configuring how to reach the actual services that will eventually handle the incoming requests.

## Configuration file

You can configure Traefik in two ways:

- The fully **dynamic** routing configuration (referred to as the **dynamic configuration**)
    - The dynamic configuration contains everything that defines how the requests are handled by your system. This configuration can change and is seamlessly hot-reloaded, without any request interruption or connection loss. 
    ```console 
    foo@bar:~$ vim /data/config/dynamic.yml
    ```

- The startup configuration (referred to as the **static configuration**)
    - Elements in the **static** configuration set up connections to providers and define the entrypoints Traefik will listen to (these elements don't change often).
    ```console 
    foo@bar:~$ vim /data/traefik.yml
    ```
## Steps to follow 

- Create a docker network
```console
foo@bar:~$ docker network create proxy-network-name
```
- Live previews
- Fullscreen mode
- Cross platform


## Author 

- [@ephraimbokuma](https://github.com/Frenchcode)
- [www.ephraimbokuma.com](https://www.ephraimbokuma.com)


