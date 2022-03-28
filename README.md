# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**
**Por Artur Poças, Daniel Silva e Rui Correia**

## Amazon Elastic beanstalk 

Aplicações implantadas na nuvem necessitam obrigatoriamente de poder de computação,memória e sistemas operativos. Criar e administrar todos estes itens podem exigir bastante trabalho e manutenção. AWS Elastic Beanstalk veio remover essa carga extra de trabalho aos programadores/empresas, poupando-lhes assim tempo e problemas na orquestração dos recursos necessários para uma implementação funcional. Uma das grandes vantagens que este serviço trouxe foi claramente permitir um maior foco no desenvolvimento e aperfeiçoamento das aplicações por parte dos programadores ao invés de se preocuparem com a gestão do ambiente que elas precisam para funcionar corretamente. 

De forma genérica o workflow  do Elastic Beanstalk está dividido em quatro etapas. A primeira passa pela criação da aplicação seguida do seu upload para o serviço da AWS. Após isso o ambiente de execução será personalizado e lançado automaticamente, por último teremos acesso à consola que permite a gestão do ambiente criado através de várias ferramentas de controlo e configuração. Podemos nesta última fase fazer updates à aplicação como escolher qual versão da mesma queremos executar.   

![workflow](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/images/clearbox-flow-00.png)

Para chegar a este objetivo o AWS Elastic Beanstalk recorre a serviços já disponibilizados pela AWS, destacando o **Amazon EC2, Elastic Load Balancing, Auto Scaling, Amazon S3, Amazon RDS e Amazon SNS**, criando o ambiente adequado para executar a aplicação. Existe sempre a possibilidade de adquirir serviços adicionais, personalizando o ambiente de acordo com as pretensões de cada cliente. 

 O AWS Elastic Beanstalk é compatível com Java, .NET, PHP, Node.js, Python, Ruby, Go, Docker, estando previsto serem integradas mais linguagens de programação no futuro. Sendo ideal para aplicações web a sua arquitetura aberta permite a integração de aplicações que não sejam web. 

Não exige nenhum custo adicional pelo seu uso, apenas são pagos os recursos subjacentes utilizados pela aplicação. 

Após o ambiente estar criado e ativo, o acesso à consola do AWS Elastic Beanstalk fica disponível dando uma visão geral do estado da aplicação. Encontra-se dividida em cinco grandes tópicos que nos permitem gerir, monitorizar e receber informação crucial sobre o funcionamento da aplicação.  
