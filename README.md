# langolier-api

API for Langolier, a personal digital garden and AI assistant.

## Usage

Requires the following environment variables:

```
DATABASE_URL=postgres://shane:shane@localhost/langolier;RUST_LOG=info
```

## NATS

This project uses NATS for messaging. To run NATS locally, use the following command:

```shell
docker run -d -p 4222:4222 --name nats-server nats:latest
```


## References

Here are reference docs for the crates used in this project:

- [axum docs](https://docs.rs/axum/latest/axum/) - web framework that focuses on ergonomics and modularity.
- [sqlx docs](https://docs.rs/sqlx/latest/sqlx/) - an async, pure Rust SQL crate featuring compile-time checked
  queries without a DSL. Supports PostgreSQL, MySQL, and SQLite.
- [tracing docs](https://docs.rs/tracing/latest/tracing/) - a framework for instrumenting Rust programs to collect
  structured, event-based diagnostic information.
- [serde docs](https://docs.rs/serde/latest/serde/) - framework for serializing and deserializing Rust data
  structures efficiently and generically.
