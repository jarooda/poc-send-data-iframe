# poc-send-data-iframe

This is a proof-of-concept (POC) for sending data between a root app and an SSO (Single Sign-On) app using iframes.

## Prerequisites
- [Node.js](https://nodejs.org/) installed
- [pnpm](https://pnpm.io/) installed globally (`npm install -g pnpm`)

## Install dependencies

```
pnpm install
```

## Running the POC

This project uses two local servers:
- **Root app**: http://localhost:3000
- **SSO app**: http://localhost:5001

To start both servers at once, run:

```
pnpm dev
```

This will serve:
- The root app from the project root at [http://localhost:3000](http://localhost:3000)
- The SSO app from the `sso/` directory at [http://localhost:5001](http://localhost:5001)

## Project Structure

```
├── index.html           # Root app entry
├── package.json         # Project config and scripts
├── sso/
│   ├── index.html       # SSO app entry
│   └── sso-button.html  # SSO button example
```

## Notes
- Make sure ports 3000 and 5001 are available.
- You can edit the HTML files to customize the POC.
