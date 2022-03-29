# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**
**Por Artur Poças, Daniel Silva e Rui Correia**
# **Resumo**<br/>
Um dos conceitos relacionados com serviços de computação na nuvem é PaaS (Platform as a Service), que normalmente de situa entre o IaaS (Infrastructure as a Service) e o SaaS (Software as a Service). <br/> É possível definir PaaS como uma categoria de serviços de computação na nuvem que fornece uma plataforma para desenvolver, implementar e executar aplicações, sem o custo e complexidade de implantação e gestão das infraestruturas necessárias. Este serviço destina-se, essencialmente, a programadores, e nele encontramos nomes como Heroku, Google App Engine ou Amazon Elastic Beanstalk. <br/> Através de plataformas como as já mencionadas, os programadores acedem a um ambiente onde estão combinados vários recursos que servem para criar aplicações e, assim, ajudar as empresas a dar resposta aos diversos desafios do dia a dia.
![PaaSEstrutura](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/Artur/paas-platform-as-a-service.png)
## **Introdução** <br/> 
Este documento serve como introdução ao conceito de PaaS (Platfrom as a Service). Para além das definições que encontramos no resumo, uma forma de melhor compreender o conceito passa por analisar exemplos práticos de implementação de soluções através do uso de plataformas. Assi, começamos por apresentar dois casos de estudo: um para a plataforma Heroku e outro para a plataforma Google App Engine. <br/> Dentro do conceito de PaaS, encontramos o Amazon Elastic Beanstalk, que é o foco principal deste documento. Como tal, o serviço da AWS é aqui apresentado através de definições, de um guia de acesso e de um caso de estudo - Prezi. 

## **Casos de Estudo**

![LogoAEStudio](https://scontent.fopo3-2.fna.fbcdn.net/v/t1.6435-9/71286345_1216414178532088_19506946889482240_n.png?_nc_cat=105&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=ngkOwX67PNAAX9dc8NV&_nc_ht=scontent.fopo3-2.fna&oh=00_AT_dNLEpq8atc7IhH26yY48_l7jhrA_63xqVF5fQrVycFw&oe=6266960E)
### **Caso de estudo de Heroku – AE Studio**

**Circunstâncias**<br/>
AE Studio é uma empresa sedeada em Los Angeles que opera na área do merchandise personalizado de celebridades. 
A plataforma interativa de merchandize permite que fãs de “Vencedores de Grammys” personalizem as suas próprias t-shirts. Para isso, são combinadas aplicações de personalização "Best Apps", impressão e envio. Graças a esta plataforma, desenvolvida e gerida com recurso a  Heroku, são garantidas Confiabilidade e Escalabilidade ao site o que permite dar resposta a milhões de utilizadores num período de dois dias. 

**Desafio**<br/>
Um músico muito famoso decide lançar um novo projeto e pretende acompanhar o lançamento com 
merchandise personalizado, pelo que contacta a AE Studio. Não é possível definir o número de visitas e 
o evento durará 48 horas. Tudo isto deve ser preparado em duas semanas. 

**Estratégia**<br/>
Graças à experiência com Heroku em projetos anteriores, a AE Studio sente confiança para 
lidar com a grande escala como comenta Ed Chen, Partner e Head Scientist, “We had no idea 
how sharp the traffic curve would be. Where Heroku really shines is that we didn’t 
have to worry about scalability, we could just focus on building the best product”. 
Algumas aplicações envolvidas neste projeto foram:
- Front-end web app; 
- Web server; 
- Job queue and order processing; 
- Print schedulling. 

**Resultados**<br/>
Durante 48 horas:
- 4,6 milhões de visualizações; 
- Cerca de 1 milhão de visitas; 
- Milhares de encomendas e ainda mais de receitas. 
Durante o evento a equipa da AE Studio esteve atenta à performance da aplicação e conseguiu,
por meio do rápido escalonamento, não só dar resposta aos picos de tráfego 
como também e reduzir os recursos e custos nos períodos de menor procura. 
Este processo resultou num enorme sucesso para a AE Studio, 
para os seus clientes Best Apps e também para a celebridade parceira. 
A título de curiosidade, a gestão das imagens neste projeto foi feita através do serviço **Amazon S3**. 


![LogoAestudio](https://futurebrandscore.com/uploads/case-studies/_heroImage/Barilla_Range.jpg) <br/> **Caso de estudo de Google App Engine - Barilla** 

**Circunstâncias**<br/> Barilla é uma empresa italiana fundada em 1877 por Pietro Barilla, que opera na área da indústria alimentar e é conhecida pela sua pasta. Em Itália, existem seis grandes unidades com cerca de 8 000 pessoas. Uma dessas unidades situa-se em Cremona e tem uma linha de produção com mais de 1 km de comprimento. O sucesso da Barilla reside muito sobre a eficiência das linhas de produção sendo este o palco dos principais desafios. 

**Desafio**<br/> O funcionamento da linha de produção é feito por três turnos rotativos sendo cada turno composto por três setores: trabalhadores de linha, chefe de turno e chefe de manutenção. Convencionalmente, cada setor possui um caderno onde são registadas as ocorrências através de anotações escritas. A informação circula depois entre setores e entre turnos pelo que não é difícil perceber o desafio existente - comunicação deficiente. 

**Estratégia**<br/> Para ajudar a resolver este desafio, a Barilla trabalhou em conjunto com a Injenia, uma empresa italiana de Tecnologias de Informação, para desenvolver uma aplicação que permitisse um sistema de mensagens prático, funcional, com possibilidade de pesquisa e para uma única versão das ocorrências. Para tal, foi usado o Google App Engine para implementar ferramentas do Google Workspace (Google Cloud SQL, Google Drive, Google Meet). 

**Resultados**<br/> *“As pessoas são sociáveis e, quando existe uma comunidade, elas começam a partilhar conhecimento e know-how. CollaborAction é um ótimo exemplo de como a colaboração social acrescenta valor a um negócio.”* Alessandra Ardriozzoia, Digital Engagement Senior Manager na Barilla <br/> No final de 2018, CollaborAction já estava implementada em 18 unidades da Barilla em todo o mundo, servindo cerca de 2700 colaboradores. Com isso a Barilla havia já recolhido mais de 50 000 posts entre os quais 20 000 fotografias e vídeos. A sua implementação em cada nova unidade demora cerca de 15 dias e o resultado está à vista e “não só aumentou a eficiência dos processos de manutenção, como também aumentou o conhecimento e compreensão que cada colaborador tem sobre o seu desempenho.” 


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

### **Prós e Contras**

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

