# Endpoint Hitter

## Introduction

Small application that is able to hit in parallel a requested endpoint, having a uuid as a path variable.
The endpoint, the methode type, the number of expected parallel requests, and the authentication credentials can be given as application parameters.

The response status for the uuid and the generated transaction id will be logged in a separate file.
Other application related logs will be sent to stdout.

For example:

We can execute a series of `POST` requests to the endpoint: `https://{env-domain}/__post-publication-combiner/{uuid}`, for the uuids read from `{uuid_file_name}.txt` (`uuid.txt` being the default).

## Installation

Download the source code, dependencies:

```sh
go build .

./endpoint-hitter [--help]
```
