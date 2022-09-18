1. Replace `<project-name>` with the name of the project

```
.devcontainer/devcontainer.json
packages/package-1/package.json
scripts/services-start-watch.sh
services/service-1/package.json
```

2. Replace `<package-1>` with the name of the first package if it exists, otherwise delete `packages/package-1` dir

```
packages/tsconfig.json
packages/package-1
packages/package-1/package.json
services/service-1/package.json
services/service-1/tsconfig.json
```

3. Replace `<service-1>` with the name of the first service if it exists, otherwise delete `services/service-1` dir

```
scripts/services-start-watch.sh
services/service-1
services/service-1/package.json
```

4. Run:

```
npm run init
```

5. To build all packages, run:

```
npm run packages-build-watch
```

6. To start all services, run:

```
npm run services-start-watch
```

7. Update `README.md` to be applicable for the current project
