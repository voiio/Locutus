# Locutus

![image](https://github.com/user-attachments/assets/6a2e49fb-eae8-4a60-a406-a1bf55bbb061)


AI orchestration for Startups

Locutus is a platform for orchestrating and running Model Context Protocol (MCP) services, enabling seamless integration of various AI and automation tools through a unified interface.

## Local Development & Testing

1. Create and configure environment variables:
   - Copy or create a `.env` file in the `mcpo/` directory and set the required environment variables for your setup.

2. Ensure required ports are free:
   - Make sure nothing else is running on ports **443** and **8000** before starting the services.

3. Start the services using Docker Compose:
   ```sh
   docker compose up
   ```

This will build and start all services as defined in `compose.yaml`.

---

### Accessing MCP Documentation

Once the server is running, you can view the documentation for any MCP service defined in `mcpo/config.json` by visiting:

```
http://localhost:8000/<mcp>/docs
```

Replace `<mcp>` with the name of the MCP service (e.g., `time`, `memory`, `freshdesk`, etc.). For example:

```
http://localhost:8000/time/docs
```
