# Actix Telemetry

This crate provides middleware for the Actix web server to support telemetry.

## Tracing

The `tracing` module offers middleware to wrap every HTTP request in a span from the `tracing` crate, allowing details to be exported via OpenTelemetry to a service such as Jaeger.

### Example

```
  let app = App::new()
      .wrap(sazzer_actix_telemetry::tracing::Span);
```
