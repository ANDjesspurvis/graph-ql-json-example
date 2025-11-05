# graph-ql-json-example
An example of a very basic graphql json DB

# graph-ql-json-example

Simple example that runs a GraphQL server from a JSON file using json-graphql-server.

## Prerequisites

- Node.js (recommended >= 14). Verify with `node -v`.
- npm (comes with Node.js)

## Quick start

1. Install dependencies

```bash
npm install
```

2. Start the server

```bash
npm start
```

This project uses `json-graphql-server` and the `db.js` file in the repository as the data source. By default the server runs on port 3000 and exposes a GraphQL endpoint at:

http://localhost:3000/graphql

You should see a console output when the server starts that confirms the port and endpoint. Open the URL in your browser to use GraphiQL (an in-browser IDE) and run queries against the sample data.

## Files

- `db.js` — sample JSON data used by `json-graphql-server` to build the GraphQL schema and resolver layer.
- `package.json` — project metadata and scripts. The `start` script launches `json-graphql-server db.js`.

## Troubleshooting

- If `npm install` fails, ensure you have a supported Node.js version and network access to the npm registry.
- If the port 3000 is already in use, stop the process using that port or restart this server on a different port by modifying how `json-graphql-server` is started (see the package docs).
- To stop the server, press Ctrl+C in the terminal where it's running.

## Notes

This README provides the minimal steps to run the example. For advanced usage and customization, see the `json-graphql-server` documentation.
