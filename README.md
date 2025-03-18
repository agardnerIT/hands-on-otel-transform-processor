# OpenTelemetry Collector: Transform Processor Hands On

Companion repo to [this video](https://example.com).

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
./o
```
