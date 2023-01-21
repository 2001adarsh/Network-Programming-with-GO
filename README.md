# Network Programming with GO

Writing contemporary network software using Go’s asynchronous features

---

### Bandwidth vs. Latency:
Network bandwidth is the amount of data we can send over a network connection in an interval of time.
A lower-bandwidth network connection may seem to have better performance than a higher-bandwidth network connection because of one characteristic: latency.

Network latency is a measure of the time that passes between sending a network resource request and receiving a response. An example of latency is the delay that occurs between clicking a link on a website and the site’s rendering the resulting page.
A website’s latency comes from several sources: the network latency between the client and server, the time it takes to retrieve data from a data store, the time it takes to compile dynamic content on the server side, and the time it takes for the web browser to render the page.

Ways to minimize latency:
- First, you can reduce both the distance and the number of hops between users and your service by using a content delivery network (CDN) or cloud infrastructure to locate your service near your users.
- Optimizing the request and response sizes will further reduce latency.
- Incorporating a caching strategy in your network applications can have dramatic effects on performance
- Finally, taking advantage of Go’s concurrency to minimize server-side blocking of the response can help

---

### Usage of bits and bytes:

A common confusion when discussing network transmission rates is using bytes per second instead of bits per second. We count the number of zeros and ones, or bits, we can transfer per second. Therefore, network transmission rates are measured in bits per second. We use bytes per second when discussing the amount of data transferred.

If your ISP advertises a 100Mbps download rate, that doesn’t mean you can download a 100MB file in one second. Rather, it may take closer to eight seconds under ideal network conditions. It’s appropriate to say we can transfer a maximum of 12.5MB per second over the 100Mbps connection.


