# What Would It Take to Get Medication for Opioid Use Disorder to More People in Need?

Svelte project code for an Urban Institute [data tool](https://apps.urban.org/features/medication-opioid-use-disorder-county-map).

Tool description: Explore how to get buprenorphine and methadone to more Michigan and New Jersey residents with opioid use disorder.

## Project credits

Research: Lisa Clemans-Cope, Doug Wissoker, Maya Payton, and Nikhil Rao

Design: Christina Baird

Development: Julia Janicki

Editing: Lauren Lastowka

Writing: Rachel Kenney

## Public URL

Production: https://apps.urban.org/features/medication-opioid-use-disorder-county-map


## Developing

To run this project locally you'll need the following installed on your local computer:

- [Node.js](https://nodejs.org/en/) >= 18.0.0
- [NPM](https://docs.npmjs.com/cli/v9/commands/npm)

Once you have Node and NPM setup, open up the project directory in a terminal and install the project dependencies by running:

```bash
npm install
```

You should now be ready to start developing! Start a local server with:

```bash
npm run dev
```

Open your browser and visit [http://localhost:5173](http://localhost:5173) to see your project running.

## Building for production

If you need to preview a production build locally, you can build your project with:

```bash
npm run build
```

This will generate a production-ready build of your project in the `dist` directory.

You can view the build you just created by running:

```bash
npm run preview
```

and opening your browser to: [http://localhost:4173](http://localhost:4173)

## Geographic data

County map files are generated with a script included in the project's Makefile. Running the following command will create the county-level topojson files needed for the project:

```bash
make src/assets/data/counties_topo.json
```
