# Traefik

This is a traefik setup template you can use to setup a reverse-proxy for all your docker containers 

## Key Concept

Traefik is based on the concept of EntryPoints, Routers, Middlewares and Services.

- **EntryPoints**:  are the network entry points into Traefik. They define the port which will receive the packets, and whether to listen for TCP or UDP.
- **Routers**: is in charge of connecting incoming requests to the services that can handle them.
- **Middlewares**: Attached to the routers, middlewares can modify the requests or responses before they are sent to your service
- **Services**: are responsible for configuring how to reach the actual services that will eventually handle the incoming requests.

## Author 

- [@ephraimbokuma](https://github.com/Frenchcode)
- [www.ephraimbokuma.com](https://www.ephraimbokuma.com)


