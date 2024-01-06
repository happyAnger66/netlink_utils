# netlink_utils

```c++
  auto netlink = NetLinkTcp::Instance();
  if (0 != netlink->GetAllSockets()) {
    return;
  }

  tcpstat ts;
  if (!netlink->GetOneSocket(local_port, peer_host, peer_port, ts)) {
    return;
  }
```