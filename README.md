# localDB 🦅

localDB is a high-performance, lightweight database built using Go (Golang). It is designed to provide fast, reliable, and scalable data storage with a focus on speed and precision. With localDB, you can achieve high throughput, low latency, and easy scalability to meet the needs of modern applications. ⚡


## Features

- ⚡ No-code platform, easy to use
- 🗄️ Based on SQLite, a lightweight database
- 🔐 Private and local first
- 📦 Can be packaged into a binary file using Bun
- 📊 Support formula field like Excel/Airtable
- 🌐 OpenAPI RESTful API support
- 🪜 Progressive deployment, from local in single file to cloud complicated stacks.
- 🐳 Supports Docker deployment
- 🛠️ Provides a UI for table management

## Screenshot

![kanban](./docs/images/kanban.jpeg)
![gallery](./docs/images/gallery.jpeg)
![calendar](./docs/images/calendar.jpeg)
![pivot](./docs/images/pivot.jpeg)
![form](./docs/images/form.jpeg)
![openapi](./docs/images/openapi.jpeg)

## Quick start

- Try [undb cloud](https://app.undb.io)

- Run with docker

```bash
docker run -p 3721:3721 ghcr.io/undb-io/undb:latest
```

## Development

### Local Development (Recommended)

1. **Install Bun**

   Refer to [Bun's official documentation](https://bun.sh/docs) for installation instructions.

2. **Clone the repository**

   ```bash
   git clone https://github.com/undb-io/undb.git
   cd undb
   ```

3. **Install dependencies**

   ```bash
   bun install
   ```

4. **Start the development server**

   ```bash
   bun run dev
   ```

### Docker compose development

```bash
docker compose up -d
```

then visit `http://localhost:3721`

## Build

### Packaging into a Binary File

1. **Build**
   ```bash
   bun run build
   ```

### Docker Deployment

1. **Build the Docker image**

   ```bash
   docker build -t undb .
   ```

2. **Run the Docker container**

   ```bash
   docker run -d -p 3721:3721 undb
   ```