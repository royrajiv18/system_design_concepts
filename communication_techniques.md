## Short Polling

- ui will consistently ask the backend for new updates.
- short live connection
- no persistent connection
- less resource utility
- problem with scale
- Ex- (real time system, notification, cricinfo, analytics, version update)
- technical implement with setInterval, and do clearInterval when navigating away or when not required anymore, also do exception handling to handle errors

## Long Polling

- ui will ask once and backend will provide all data at once
- single long lived connection
- connection is open until you get new data/timeout
- cons: large number of connection, more the load
- ex- real time collaboration

## Web Socket

- ui don't have to wait for entire data to get ready, next request can also be sent in between, ex-whatsapp
- full duplex communication
- single long live tcp connection
- continuous and bidirectional communication
- Ex- (Analytics, Financial Trading, online gaming, collab like google doc, )
- challenges - resource usage, connection limits, sticky session, load balancer, authentication, firewall, scaling, debugging/testing, backward compatibility, resource cleanup

## SSE (Server side events)

- based on some events, backend will give data
- long live unidirectional communication
- single http connection
- use lib eventSource
- Ex - (feeds, notifications, monitoring dashboard)
- challenges - browser compatibility, connection limit, connection timeout, background tab behavior, resource utilization, load balancer, sticky connection, proxy firewall, testing, broadcasting

## Web hooks

- once your request is done, some actions are made from backend
- Real time communication
- Event driven
- POST REST API(payload, authorization, secret)
- Retry
- verification/acknowledge
- Ex- notification system, data synchronization, automation, (in github)
