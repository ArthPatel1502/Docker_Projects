# Distortless Docker Calculator

A simple command-line calculator written in Go and packaged using a multi-stage Docker build. The final image uses `scratch`, resulting in a small and secure container image.

## Features

- Supports basic arithmetic operations
- Built with Go
- Multi-stage Docker build for minimal image size

## Build

```bash
docker build -t distortless-calculator .
```

## Run

```bash
docker run -it distortless-calculator
```

Follow the on-screen prompt and enter expressions such as:

```text
1 + 2
5 * 7
```

## Project Structure

- `calculator.go` – Calculator source code
- `Dockerfile` – Multi-stage Docker build configuration
