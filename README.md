# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**
**Por Artur Poças, Daniel Silva e Rui Correia**

##Amazon Elastic beanstalk 

Aplicações implantadas na nuvem necessitam obrigatoriamente de poder de computação,memória e sistemas operativos. Criar e administrar todos estes itens podem exigir bastante trabalho e manutenção. AWS Elastic Beanstalk veio remover essa carga extra de trabalho aos programadores/empresas, poupando-lhes assim tempo e problemas na orquestração dos recursos necessários para uma implementação funcional. Uma das grandes vantagens que este serviço trouxe foi claramente permitir um maior foco no desenvolvimento e aperfeiçoamento das aplicações por parte dos programadores ao invés de se preocuparem com a gestão do ambiente que elas precisam para funcionar corretamente. 

De forma genérica o workflow  do Elastic Beanstalk está dividido em quatro etapas. A primeira passa pela criação da aplicação seguida do seu upload para o serviço da AWS. Após isso o ambiente de execução será personalizado e lançado automaticamente, por último teremos acesso à consola que permite a gestão do ambiente criado através de várias ferramentas de controlo e configuração. Podemos nesta última fase fazer updates à aplicação como escolher qual versão da mesma queremos executar.   

![workflow](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/images/clearbox-flow-00.png)
