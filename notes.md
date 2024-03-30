### Ports and Adapters


* Crescimento sustentável
* Sofrware precisa se pagar ao passar do tempo
* Software deve ser desenhado por você e não pelo seu framework

> Arquitetura diz respeito com o futuro do seu software CRUD qualquer um faz




##### Ciclo de vida de muitos projetos

Fase 1  | Fase 2  | Fase 3 | Fase 4 | fase 5 | Fase 6 | Fase 7 | Fase 8 | Fase 9 | Fase 10
:--------| :-------: | :---------: | :---------:| :---------:| :---------:| :---------: | :---------: | :---------: | :---------:
Banco de dados | Regras de negócio | Mais acessos | Mais acessos | Escala horizontal | GraphQL | Inconsistência CRM | Microsserviços | Kubernets | Use a IMAGINAÇÃO
Cadastros | Criação de APIs | Upgrades hardware | Upgrade hardware | Sessões | Bugs constantes | Containers | DB compartilhado | CI/CD
Validações | Consumo de APIs | Cache | BD Ralatórios | Uploads | Logs? Ops | CI/CD | Problemas com tracing | Mensageria
Servidor Web | Autorização | API parceiros | Comandos | Refatoração | Integração CRM | Memória | Lentidão | Perda de mensagens
Controllers | Relatórios | Regras parceiros | V2 da API | Autoscaling | Migração para **React** | Logs | Custo elevado | Consultorias
Views | Logs | Relatórios | |CI/CD | | se livrar do legado
Autenticação |  |
Upload de arquivos



#### Principais problemas

* Visão de futuro
* Limites bem definidos
* Troca e adição de componentes
* Escala
* Otimizações frequentes
* Preparado para mudanças

#### Reflexões

* Está sendo doloroso para o desenvolvedor?
* Poderia ser evitado?
* Software está se pagando?
* Será que a relação com o cliente está boa?
* Cliente terá prejuízo com a brusca mudança arquitetural?
* Em qual momento tudo se perdeu?
* Se você fosse novo na equipe, você julgaria os devs que fizeram isso?


#### Arquitetura Hexagonal ou "Ports and Adapters"

* Definição de limites e proteção nas regras da aplicação
* Componentização e desacoplamento
    * Logs
    * Cache
    * Upload
    * Banco de dados
    * Comandos
    * Filas
    * HTTP / APIs / GraphQL
* Facilidade na quebra para microsserviços

 ##### Lógica básica

- Aplicação (centro)
- Cliente (esquerdo)
- Servidor(direito)


dentro = aplicação
fora  =  cliente e servidor

 - Fora(esquerdo)
    * REST
    * CLI
    * RPC
    * GraphQL
    * UI
 - Fora (direito)
    * DB
    * Redis
    * Filesystem
    * Lambda
    * API


### Observações

* Não há um padrão de estabelecido de como o código deve ser organizado



