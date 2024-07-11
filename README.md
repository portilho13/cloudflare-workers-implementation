# Cloudflare Workers Implementation

This is a basic implementation of Cloudflare Workers, a serverless platform running on the edge.

| Service                                        | Description                          | Stack       | Status       |
|------------------------------------------------|--------------------------------------|-------------|--------------|
| [Proxy](https://github.com/portilho13/worker-proxy) | Reverse Proxy with DDos                              | Rust  | In Progress  |
| [Client](https://github.com/portilho13/worker-client) | Client used to upload projects            | Rust  | In Progress      |
| [Main](https://github.com/portilho13/worker-main)                                 | Main server resembling an ISP         | Go  | In Progress  |
| [Worker](https://github.com/portilho13/worker)                                 | Worker Server        | Rust  | In Progress  |

## Current Supported Framworks

- React
- Angular

## Current Features

### Proxy:
- Basic reverse proxy functionality
- DDos protection with current ratelimiting mechanism.

### Client
- Client is able to map all content of dirs, subdirs and files.
- Client is able to send project over TCP connection

### Main
- Main is able to create TCP connection with all workers.
- Main is able to create TCP connection with client.
- Main is able to redirect project content sended by the client to all workers.

### Worker

- Worker is able to stablish TCP connection with Main.
- Workers is able to recive project content.
- Workers is able to mount the project.
- Workers is able to run the project.
