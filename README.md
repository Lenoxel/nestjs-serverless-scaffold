# Projeto Base - Nest.js | Serverless
Esse é o projeto base para iniciar com Nest.js e Serverless Framework

## Como usar
### Preparação

```
Caso ainda não tenha instalado: $ npm install @nestjs/cli serverless -g

$ git clone https://github.com/Lenoxel/nestjs-serverless-scaffold.git 【projectName】
$ cd 【projectName】
$ npm install
$ npm start
```

### Desenvolvimento
#### Usando o NestCLI

```
$ npm start
```

```
$ npm start

> scaffold-nestjs-serverless@0.0.1 start C:\Codes\js_codes\scaffold-nestjs-serverless
> nest start

[Nest] 13340   - 2020-08-13 13:04:31   [NestFactory] Starting Nest application...
[Nest] 13340   - 2020-08-13 13:04:31   [InstanceLoader] AppModule dependencies initialized +17ms
[Nest] 13340   - 2020-08-13 13:04:31   [RoutesResolver] AppController {}: +6ms
[Nest] 13340   - 2020-08-13 13:04:31   [RouterExplorer] Mapped {, GET} route +7ms
[Nest] 13340   - 2020-08-13 13:04:31   [NestApplication] Nest application successfully started +3ms
```

Acesse o projeto por - http://localhost:3000

#### Usando o serverless-offline
__Antes, rode o comando: `npm run build`__

```bash
$ sls offline
```

```
$ sls offline
Serverless: DOTENV: Loading environment variables from :
Serverless: Compiling with Typescript...
Serverless: Using local tsconfig.json
Serverless: Typescript compiled.
Serverless: Watching typescript files...
offline: Starting Offline: dev/us-west-2.

...

offline: [HTTP] server ready: http://localhost:3000
```

Acesse o projeto por - http://localhost:3000

#### Usando o Swagger para desenvolvimento

```
$ npm run start:swager
```

```
> scaffold-nestjs-serverless@0.0.1 start:swagger C:\Codes\js_codes\scaffold-nestjs-serverless
> npx ts-node src/swagger.ts

[Nest] 8908   - 2020-08-13 13:10:02   [NestFactory] Starting Nest application...
[Nest] 8908   - 2020-08-13 13:10:02   [InstanceLoader] AppModule dependencies initialized +16ms
[Nest] 8908   - 2020-08-13 13:10:02   [RoutesResolver] AppController {}: +90ms
[Nest] 8908   - 2020-08-13 13:10:02   [RouterExplorer] Mapped {, GET} route +2ms
[Nest] 8908   - 2020-08-13 13:10:02   [NestApplication] Nest application successfully started +4ms
```

Acesse o projeto por - http://localhost:3001/api