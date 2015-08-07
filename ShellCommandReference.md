# Shell Commands for Reference

## SSH
### Local Port Forwarding or Outbound Tunnelling
```
ssh -L username@intermediateserver.com localPort:destinationServer:destinationport -p alternateSSHPortOnDestinationServer
```

### Remote Port Forwarding or Inbound Tunnelling
