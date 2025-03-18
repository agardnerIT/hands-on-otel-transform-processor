# OpenTelemetry Collector: Transform Processor Hands On

Companion repo to [this video](https://www.youtube.com/watch?v=budS405GGds).

[![OpenTelemtry transform processor video](https://img.youtube.com/vi/budS405GGds/0.jpg)](https://www.youtube.com/watch?v=budS405GGds)

[Download the OpenTelemetry contrib collector](https://github.com/open-telemetry/opentelemetry-collector-releases/releases) (or bring your own distribution) - as long as it contains the `transform`, `resourcedetection` and `batch` processors.

## Start the Backend

I use [OpenObserve](https://github.com/openobserve/openobserve/releases/tag/v0.14.4) in this video but you can use any Observability backend that accepts OpenTelemetry data. If your Observability system does not accept OpenTelemetry, get a new one. OpenTelemetry is the future and any future-proof solution should fully support OTEL.

```
./openobserve
```

## Get the API Token and Start the Collector
Follow the video to find the API token and store as an environment variable called `OPEN_OBSERVE_KEY` - the collector requires this to send data to OpenObserve.

```
export OPEN_OBSERVE_KEY=TODO
./otelcol-contrib --config=scenario1.yaml

./otelcol-contrib --config=scenario2.yaml

./otelcol-contrib --config=scenario3.yaml

./otelcol-contrib --config=scenario4.yaml

./otelcol-contrib --config=scenario5.yaml

./otelcol-contrib --config=scenario6.yaml

./otelcol-contrib --config=scenario7.yaml

./otelcol-contrib --config=scenario8.yaml

./otelcol-contrib --config=scenario9.yaml
```
