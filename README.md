# Quarkus GCP Template

This template provides a starting point for building Java applications with [Quarkus](https://quarkus.io/), [Gradle](https://gradle.org/), and [GraalVM](https://www.graalvm.org/) using [jOOQ](https://www.jooq.org/) with a PostgreSQL database. The project is ready to be containerized and deployed to Google Cloud Platform (GCP), for example to Cloud Run.

## Features

- **Quarkus** framework with RESTEasy Reactive for building REST APIs
- **Gradle** build tool
- **GraalVM** native image support
- **jOOQ** for type-safe database access
- **PostgreSQL** as the example database
- Sample REST endpoint `GET /hello`

## Running locally

```bash
gradle quarkusDev
```

## Building a native executable

```bash
gradle build -Dquarkus.package.type=native
```

The resulting executable can be deployed to GCP (e.g. Cloud Run). Consult the [Quarkus GCP guide](https://quarkus.io/guides/deploying-to-google-cloud) for deployment steps.
