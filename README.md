----------RUN ./build/dartserver-----------------
Running 30s test @ thhp://127.0.0.1:8080
  12 threads and 300 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    36.31ms   46.98ms   1.04s    98.64%
    Req/Sec   781.46     98.13     1.01k    88.10%
  275258 requests in 30.03s, 65.63MB read
Requests/sec:   9166.75
Transfer/sec:      2.19MB


----------RUN DOCKER------------------------------745MB
Running 30s test @ http://localhost:8080
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    41.23ms   78.50ms   1.25s    98.40%
    Req/Sec     1.01k   334.62     1.90k    59.88%
  359935 requests in 30.05s, 85.82MB read
Requests/sec:  11976.43
Transfer/sec:      2.86MB


----------RUN DOCKER MULTISTAGE----------------- 75.5MB
Running 30s test @ http://localhost:8080
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    44.83ms   66.32ms   1.14s    98.74%
    Req/Sec     0.85k   172.30     2.26k    76.08%
  305446 requests in 30.09s, 72.82MB read
Requests/sec:  10152.58
Transfer/sec:      2.42MB
