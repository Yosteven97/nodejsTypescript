#use TypeScript using Node.js
1. npm install -g typescript
2. tsc --init
3. open tsconfig.json and replace with 
{
  "compilerOptions": {                        
    "target": "es6",                               
    "module": "commonjs",                           
    "outDir": "./dist",                             
    "rootDir": "./src",                             
    "strict": true,
    "moduleResolution": "node",
    "esModuleInterop": true,                       
  },
  "exclude":[
    "./node_modules"
  ]
}
4. npm install -D typescript
5. run tsc on terminal folder root
6. node dist/index.js
7. npm install -D ts-node
8. configure your package.json with 
"scripts": {
   "start": "ts-node ./src/index.ts"
}
9. run npm start 

#using typescript with packages, example with express.js
10. npm install -D @types/node
11. npm install -D @types/express
12. open http://localhost:8000/ on your browser
