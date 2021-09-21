### Instalação do NestJS Cli
```
npm i -g @nestjs/cli
```

### Criação do projeto
```
nest new <project-name>
```

### Criação de um módulo
@Module({controllers: [], providers: [...services]})
```
nest g module <module_name>
```

### Criação de um controlador
@Controller('api/v1/examplepath')

Definimos uma rota e os métodos para lidar com as requisições.
```
nest g controller <controller_name>
```

### Criação de um serviço
@Injectable()

Concentra a lógica de negócio.
```
nest g service <service_name>
```

### NestJS Pipes (data and parameters validation)
Act on the arguments that will be processed by the route handler, just before the handler is called.

They can transform or validate data, and throw exceptions.

Applied into DTOs.
```
npm i class-validator class-transformer
```

Then, into controllers:

@UsePipes(ValidationPipe)