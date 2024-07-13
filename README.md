# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Running the site locally

### Installation

```shell
npm install
```

### Local Development

```shell
npm start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```shell
npm run build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service. If you want to test out the statically build content locally, you can use:

```shell
npm run serve
```

### Local Search

This site uses a local search engine that generates an index of the site at build time and downloads it to the browser
for the user to do searches. This avoids using a separate search service and will work well as long as the size of the
site is relatively small (meaning the index size stays small). The initial size of the index is 58kb, but it should be
monitored over time. Netlify will cache files so as long as the index hasn't changed, the browser shouldn't redownload
the file.

The local search is not available when you are running local development using `npm start`. To try out the search
locally, you'll need to do a `npm run build` followed by a `npm run serve`. This will build the static content
(like for Netlify) locally, then serve it up using a local web server, but not watch for changing files. If you run
in a development mode, the search box will be grayed out.
