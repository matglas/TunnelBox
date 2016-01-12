# Usage

Through several environment params you can setup a connection.

- SSH_USER
- SSH_HOST
- TUNNEL_PORT
- TARGET_HOST
- TARGET_PORT

Run docker run -e "SSH_USER=root" -e "SSH_HOST=example.com" -e "TUNNEL_PORT=3012" -e "TARGET_HOST=localhost" -e "TARGET_PORT=3001"  -p 3012:3012 -d matglas/TunnelBox:latest

- The SSH_* is used to setup a secure connection to the host from which you want to tunnel.
- The TUNNEL_PORT is used to define the port that needs to be exposed by SSH to tunnel on.
- The TARGET_* is used to define where to connect to from the SSH host you connect to.