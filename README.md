{
  "version": 1,
  "sdk_version": "3.0.4",
  "path": "/functions/v1/mcp",
  "auth": {
    "type": "none"
  },
  "mcp": {
    "server": {
      "name": "order-scan-dine-pay",
      "version": "0.1.0",
      "title": "order-scan-dine-pay"
    },
    "tools": [
      {
        "name": "list_menu",
        "title": "List menu",
        "description": "List dishes on the restaurant menu, optionally filtered by category.",
        "annotations": {
          "readOnlyHint": true,
          "idempotentHint": true,
          "openWorldHint": false
        },
        "inputSchema": {
          "type": "object",
          "properties": {
            "category": {
              "type": "string",
              "description": "Category name, e.g. Starters."
            }
          },
          "additionalProperties": false,
          "$schema": "http://json-schema.org/draft-07/schema#"
        },
        "outputSchema": null
      }
    ]
  }
}
