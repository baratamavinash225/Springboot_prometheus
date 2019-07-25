Prometheus installation is simple and easy with docker, we can install in just single command. It runs on the port 9090 by default and hence we pass it in docker command to expose to host network.

Sample docker run with out any custom configurations:

docker run -d -p 9090:9090 prom/prometheus

You can verify the installation on http://localhost:9090 where prometheus UI is running. By default you can find some metrics and the graphs that are available in the UI. You can look at the http://localhost:9090/metrics to see what all the default types of metrics available.

In our example, goal is to print the count of number of requests that hit to the Spring REST API and produce as a metrics, hence we need to make few modifications in the yml file which is available in this folder.


Under the scrape_configs we need to make our changes, parameters that are changed are:
metrics_path
targets - where Spring Application is running, in our case we have launched on http://localhost:8080/

Metrics are written into http://localhost:8080/prometheus-metrics.

Modified configuration and the docker command is available in the file.

