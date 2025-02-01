# Profiler Renderservice

The Frontend for the Profiler App

## Attributions

- The [Vue.js Team](https://vuejs.org/) for creating my favorite frontend Framework
- The [PrimeVue Team](https://primevue.org/) for creating my favorite vue UI Library

## What you'll need

- [Nodejs](https://nodejs.org/)
- JavaScript toolkit like [npm](https://www.npmjs.com/), [bun](https://www.bun.sh/), or [pnpm](https://pnpm.io/)

## Things I recommend

- [WSL](https://learn.microsoft.com/en-us/windows/wsl/install/Linux) (Because I built a few helper-scripts to get you started)
- [bun](https://www.bun.sh/) (Because it's performance is staggering and how easy it is to use)

## How to run it

Either you use `bun run dev`, or if you want to debug in VSCode, you can use the following Launch Configuration: 

```json
//Chrome
{
    "type": "chrome",
    "request": "launch",
    "name": "Client: Chrome",
    "url": "http://localhost:5173",
    "webRoot": "${workspaceFolder}/frontend"
}
//Edge
{
    "type": "msedge",
    "request": "launch",
    "name": "Client: Edge",
    "url": "http://localhost:5173/",
    "webRoot": "${workspaceFolder}/frontend",
    "sourceMaps": true,
    "sourceMapPathOverrides": {
        "meteor://💻app/*": "${webRoot}/*",
        "webpack:///./~/*": "${webRoot}/node_modules/*",
        "webpack://?:*/*": "${webRoot}/*"
    },
},
```