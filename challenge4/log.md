<h1>My Adventures in Upscaling</h1>
<p>My first venture into the Stats page revealed a hostname of "70ac89f69e7a"</p>
<p>Repeated viewings showed the hostname remained consistent.</p>
<h2>Scaling Up</h2>
<p>Scaling up to multiple instances was as easy as running the compose file with the <b>--scale</b> flag.</p>
<p>With the newly upscaled node instances, the compose ps list looked a little something like this:</p>

| CONTAINER ID | IMAGE | COMMAND | CREATED | STATUS | PORTS | NAMES |
| ------------ | ----- | ------- |-------- | ------ | ----- | ----- |
| bf0bcbdbda69 | docker-node-service | docker-entrypoint.sh... | 33 seconds ago | Up 21 seconds | 0.0.0.0:65181->3000/tcp | docker-node-service-3 |
| 517b8b942c6e | docker-node-service | docker-entrypoint.sh... | 33 seconds ago | Up 21 seconds | 0.0.0.0:65182->3000/tcp | docker-node-service-1 |
| b264cb9026bb | docker-node-service | docker-entrypoint.sh... | 33 seconds ago | Up 21 seconds | 0.0.0.0:65183->3000/tcp | docker-node-service-2 |
| 2508bb80c4c6 | docker-nginx        | /docker-entrypoint....  | 2 minutes ago  | Up 2 minutes  | 0.0.0.0:8080->80/tcp    | docker-nginx-1       |
| eed78586fae6 | mariadb             | docker-entrypoint.sh... | 2 minutes ago  | Up 2 minutes  | 0.0.0.0:3306->3306/tcp  | mariadb              |
