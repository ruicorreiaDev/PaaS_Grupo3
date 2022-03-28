# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**
**Por Artur Poças, Daniel Silva e Rui Correia**

## **Sobre Amazon Elastic Beanstalk** 

Aplicações implantadas na nuvem necessitam obrigatoriamente de poder de computação,memória e sistemas operativos. Criar e administrar todos estes itens podem exigir bastante trabalho e manutenção. AWS Elastic Beanstalk veio remover essa carga extra de trabalho aos programadores/empresas, poupando-lhes assim tempo e problemas na orquestração dos recursos necessários para uma implementação funcional. Uma das grandes vantagens que este serviço trouxe foi claramente permitir um maior foco no desenvolvimento e aperfeiçoamento das aplicações por parte dos programadores ao invés de se preocuparem com a gestão do ambiente que elas precisam para funcionar corretamente. 

### **Como Funciona**
De forma genérica o workflow  do Elastic Beanstalk (ver figura 1) está dividido em quatro etapas. A primeira passa pela criação da aplicação seguida do seu upload para o serviço da AWS. Após isso, o ambiente de execução será personalizado e lançado automaticamente, por último teremos acesso à consola que permite a gestão do ambiente criado através de várias ferramentas de controlo e configuração. Podemos nesta última fase fazer updates à aplicação como optar qual versão da mesma queremos executar.   

![workflow](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/images/clearbox-flow-00.png)

Figura 1 - Esquema do workflow do AWS Elastic Beanstalk 

Para chegar a este objetivo o AWS Elastic Beanstalk recorre a serviços já disponibilizados pela AWS, destacando o **Amazon EC2, Elastic Load Balancing, Auto Scaling, Amazon S3, Amazon RDS e Amazon SNS**, criando o ambiente adequado para executar a aplicação. Existe sempre a possibilidade de adquirir serviços adicionais, personalizando o ambiente de acordo com as pretensões de cada cliente. 

 O AWS Elastic Beanstalk é compatível com Java, .NET, PHP, Node.js, Python, Ruby, Go, Docker, estando previsto serem integradas mais linguagens de programação no futuro. Sendo ideal para aplicações web a sua arquitetura aberta permite a integração de aplicações que não sejam web. 

Não exige nenhum custo adicional pelo seu uso, apenas são pagos os recursos subjacentes utilizados pela aplicação. 

Após o ambiente estar criado e ativo, o acesso à consola do AWS Elastic Beanstalk fica disponível dando uma visão geral do estado da aplicação. Esta encontra-se dividida em cinco grandes tópicos que nos permitem gerir, monitorizar e receber informação crucial sobre o funcionamento da aplicação.  

- **Configuração** - Visão geral dos recursos criados para o ambiente, podendo efetuar alterações tais como mudar o serviço de auto-scaling, tipo de instâncias do EC2, ativar e desativar notificações; 

- **Health** - Mostra o estado e as informações detalhadas de integridade sobre as instâncias do Amazon EC2 que executam a aplicação; 

- **Monitorização** - Permite o acesso a estatísticas do ambiente como a latência e utilização de CPU. Pode ser usada para a criação de alarmes segundo métricas personalizadas. 

- **Eventos** – Mostra informações ou mensagens de erro dos serviços que estejam a ser utilizados no ambiente; 

- **Tags** - Permitem categorizar os recursos da AWS de diferentes formas (por finalidade, por utilizador ou por ambiente), facilitando assim a sua rápida identificação. 

Com uma perspetiva geral do funcionamento e finalidade do serviço Elastic Beanstalk é possível fazer uma análise dos prós e contras. 

**Prós** 

- **Fácil acesso** - É a forma mais rápida e simples de implementar uma solução de ambiente para uma aplicação na AWS; 

- **Custo** - Não existe custo adicional pelo uso do serviço; 

- **Flexibilidade** - Permite a personalização manual de cada ferramenta; 

- **Produtividade** - Gestão da infraestrutura automatizada, permite poupança de tempo para o desenvolvimento da aplicação. 

**Contras** 

- **Difícil diagnóstico de problemas** – Em caso de alguma falha no serviço, sendo ele gerido automaticamente, torna mais complicado a tarefa da procura pela origem do problema;  

- **Updates automáticos** - Embora possa aparentar ser uma vantagem e na maioria dos casos assim o é, noutros, os updates automáticos podem causar problemas na execução da aplicação; 

- **Falta de controlo detalhado** - Apesar das possibilidades pré-definidas serem vastas, nem sempre são suficientes para todos os casos de uso.
