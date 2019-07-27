# Istio Proxy

The Istio Proxy is a microservice proxy that can be used on the client and server side, and forms a microservice mesh. The Proxy supports a large number of features.

Client Side Features:
客户端功能

- *Discovery & Load Balancing*. The Proxy can use several standard service discovery and load balancing APIs to efficiently distribute traffic to services.

- *Credential Injection*. The Proxy can inject client identity, either through connection tunneling or protocol-specific mechanisms such as JWT tokens for HTTP requests.

- *Connection Management*. The Proxy manages connections to services, handling health checking, retry, failover, and flow control.

- *Monitoring & Logging*. The Proxy can report client-side metrics and logs to the Mixer.

Server Side Features:
服务端功能

- *Rate Limiting & Flow Control*. The Proxy can prevent overload of backend systems and provide client-aware rate limiting.
- *速率限制与流量控制*. 代理可以避免后端系统过载并提供客户端的速率限制的能力.

- *Protocol Translation*. The Proxy is a gRPC gateway, providing translation between JSON-REST and gRPC.
- *协议转换*. 代理的默认是gRPC网关, 提供JSON-REST 和 gRPC间的协议转换

- *Authentication & Authorization*. The Proxy supports multiple authentication mechanisms, and can use the client identities to perform authorization checks through the Mixer.
- *认证与授权*. 代理提供了多种认证机制，并能够通过Mixer来完成客户端身份认证并进行权限检查

- *Monitoring & Logging*. The Proxy can report server-side metrics and logs to the Mixer.

Please see [istio.io](https://istio.io)
to learn about the overall Istio project and how to get in touch with us. To learn how you can
contribute to any of the Istio components, including the proxy, please 
see the Istio [contribution guidelines](https://github.com/istio/istio/blob/master/CONTRIBUTING.md).
