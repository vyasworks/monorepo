# monorepo

Objectives: 

1. Checkout Yarn 2 / Berry
   1. Zero Installs
   2. PnP
   3. What is it? 
   4. Complexities 
   5. Are any projects using this? 
2. Lerna and Mono repo 
3. Lambda build with dependencies. 

1. Yarn 2 - Berry

Zero Installs - https://yarnpkg.com/features/zero-installs
PnP - https://yarnpkg.com/features/pnp

### So, What is it? 

1. Essentially PnP + Zero Installs enables a project to work out of the box, without having to do yarn || yarn install 
2. All the magic is in `.pnp.cjs` file and in `.yarn/cache`
3. Instead of letting Node do the module resolution using https://nodejs.org/api/modules.html#all-together this algorithm, yarn wants to manage dependencies resolution. 
4. Benefits - Time, Space, Efficiency, Less errors etc.. More on the Yarn 2 website. 
5. Cons - Packges dont support PnP out of the box, VS code cannot directly resolve and help on intellisense, TS doesn't have native support. All WIP. some plugins exist to make things work. 

### So were you able to do it? 

No. I could not get VS code to work with Yarn 2 PnP yet. 
No. I could not get the app to start properly. 

### So, why use it at all.. 

1. Yarn cache
2. node_module linker backwards compatible 
3. can become zero installs in the future, once there is better support. 
4. Fast CI CD 
