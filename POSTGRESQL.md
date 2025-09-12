# PostgreSQL Extension

This document provides instructions for the Gemini agent to assist users with the PostgreSQL extension.

## PostgreSQL MCP Server (Data Plane: Connecting and Querying)

This section covers connecting to a PostgreSQL database instance.

1.  **Verify Environment Variables**: Before attempting to connect, confirm with the user that the following environment variables are set in the extension configuration or their shell environment.

    *   `POSTGRES_HOST`: The hostname or IP address of the PostgreSQL server.
    *   `POSTGRES_PORT`: The port number of the PostgreSQL server.
    *   `POSTGRES_DATABASE`: The name of the database to connect to.
    *   `POSTGRES_USER`: The username for authentication.
    *   `POSTGRES_PASSWORD`: The password for authentication.

2.  **Handle Missing Variables**: If a command fails with an error message containing a placeholder like `${POSTGRES_HOST}`, it signifies a missing environment variable. Inform the user which variable is missing and instruct them to set it.

3.  **Handle Permission Errors**: If you encounter permission errors, ensure the user has the correct privileges on the PostgreSQL database.
