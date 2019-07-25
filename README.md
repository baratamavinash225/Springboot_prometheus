# Springboot Prometheus
This application is to integrate spring boot with the prometheus. Simple use case is to generate a metrics on prometheus as how many requests has hit to the spring boot application

<h3>Components involved:</h3>

1. Prometheus
2. Spring Boot
3. Docker

<h4>Prometheus:</h4>
<p>Prometheus is an open-source systems monitoring and alerting toolkit originally built at SoundCloud.Prometheus scrapes metrics from instrumented jobs, either directly or via an intermediary push gateway for short-lived jobs. It stores all scraped samples locally and runs rules over this data to either aggregate and record new time series from existing data or generate alerts. Grafana or other API consumers can be used to visualize the collected data.</p>

<h4>Spring Boot:</h4>
<p>Spring Boot makes it easy to create stand-alone, production-grade Spring based Applications that you can "just run". In this app, we have used to create a rest service and the end users can hit the rest URL to post. In real world,there could be any kind of application, but since the idea is to push metrics and hence we didn't concentrate much on spring boot</p>

<h4>Docker</h4>
<p>Docker is a set of coupled software-as-a-service and platform-as-a-service products that use operating-system-level virtualization to develop and deliver software in packages called containers. The software that hosts the containers is called Docker Engine.We have used docker here to launch prometheus instead of going into traditional installation.</p>

