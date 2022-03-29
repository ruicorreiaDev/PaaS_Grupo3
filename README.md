# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**
**Por Artur Poças, Daniel Silva e Rui Correia**
## **Resumo**<br/>
Um dos conceitos relacionados com serviços de computação na nuvem é PaaS (Platform as a Service), que normalmente se situa entre o IaaS (Infrastructure as a Service) e o SaaS (Software as a Service). <br/> É possível definir PaaS como uma categoria de serviços de computação na nuvem que fornece uma plataforma para desenvolver, implementar e executar aplicações, sem o custo e complexidade de implantação e gestão das infraestruturas necessárias. Este serviço destina-se, essencialmente, a programadores, e nele encontramos nomes como Heroku, Google App Engine ou Amazon Elastic Beanstalk. <br/> Através de plataformas como as já mencionadas, os programadores acedem a um ambiente onde estão combinados vários recursos que servem para criar aplicações e, assim, ajudar as empresas a dar resposta aos diversos desafios do dia a dia.
![PaaSEstrutura](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/Artur/paas-platform-as-a-service.png)
## **Introdução** <br/> 
Este documento serve como introdução ao conceito de PaaS (Platfrom as a Service). Para além das definições que encontramos no resumo, uma forma de melhor compreender o conceito passa por analisar exemplos práticos de implementação de soluções através do uso de plataformas. Assim, começamos por apresentar dois casos de estudo: um para a plataforma Heroku e outro para a plataforma Google App Engine. <br/> Dentro do conceito de PaaS, encontramos o Amazon Elastic Beanstalk, que é o foco principal deste documento. Como tal, o serviço da AWS é aqui apresentado através de definições, de um caso de estudo - Prezi e de um guia de configuração passo a passo (tutorial).

## **Casos de Estudo PaaS**

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


![LogoAestudio](https://futurebrandscore.com/uploads/case-studies/_heroImage/Barilla_Range.jpg)
### **Caso de estudo de Google App Engine - Barilla** 

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

![Logoprezi](https://assets.prezicdn.net/assets-versioned/coverservice-versioned/2972-da8bc85/common/img/prezi-logo-for-share.png)
### Caso de Estudo – Prezi

**Circunstâncias**<br/>
Fundada em 2009, Prezi é uma empresa que desenvolve software de apresentações baseado em computação na nuvem. A sua missão é reinventar o método de criar apresentações ao oferecer, aos utilizadores, as ferramentas necessárias para organizar claramente as ideias pretendidas e apresentá-las da forma mais cativante e interativa possível.

**Desafio**<br/>
Para ser capaz de acompanhar o crescimento acentuado, a Prezi precisava de uma plataforma em cloud, com grande capacidade de escalabilidade e automação, que hospedasse o seu software como um serviço. Era crítico, também, que a plataforma fosse flexível, intuitiva e fácil de gerir, para que os developers pudessem rapidamente criar novas funcionalidades para os clientes. Além do mais, a empresa precisava de uma plataforma cloud capaz de oferecer a maior confiabilidade possível, que servisse os mais de 1 milhão de novos clientes que aderem ao Prezi por mês.

Os trabalhadores da Prezi também necessitavam de uma maneira rápida de analisar e visualizar dados para que pudessem melhorar a oferta dos seus serviços. Contudo, quando os trabalhadores precisavam de informação, era-lhes exigido contactar com a equipa de dados, que por sua vez escreviam código específico para cada caso, movendo manualmente os dados para uma tabela de forma a fazer análise. Com tantos pedidos a surgir de diferentes partes da empresa, a equipa de dados normalmente acumulava serviço, demorando por vezes dias a dar resposta.

**Estratégia (Porquê AWS?)**<br/>
Nos primeiros anos de negócio, a Prezi hospedava as suas ferramentas de apresentação interativas numa plataforma gerida em cloud, com muitos dos seus serviços desenvolvidos on-premises. A organização eventualmente começou a migrar os seus SaaS para a Amazon Web Services (AWS) em 2012 por causa da alta escalabilidade da plataforma.

A Prezi foi também atraída pela AWS por causa do serviço Amazon Redshift, uma solução de armazenamento de dados que permite a análise de uma forma simples e com elevado custo-benefício. A empresa pretendia que todos os empregados fossem capazes de aceder a dados sem terem de esperar pela ajuda da equipa especializada em dados. Além do mais a Prezi queria tornar simples o processo de visualização de dados para que fosse possível, rapidamente, detetar tendências e ajustar os seus produtos com base no que é procurado pelos clientes.

Além do Redshift, a Prezi depende de outros componentes de base de dados AWS incluindo Amazon Relational Database Service (Amazon RDS) para operar e escalar o servidor SQL na cloud; Amazon DynamoDB, para armazenar metadados e mover dados entre aplicações; Amazon ElastiCache para implementar, operar e escalar uma in-memory cache na cloud; e Amazon Simple Storage Service (Amazon S3) para armazenar apresentações de utilizadores e servir de back up para as outras bases de dados da empresa.

Para análise, a Prezi utiliza Amazon Elastic MapReduce (Amazon EMR), que permite aos developers processar de forma simples e eficiente grandes quantidades de dados. Para computação, a organização usa instâncias da Amazon Elastic Compute Cloud (Amazon EC2). A Prezi depende de AWS Config para segurança e gestão. Esse serviço rastreia as alterações de configuração aos recursos do Prezi no AWS e envia notificações sempre que os recursos são criados, alterados ou apagados. A Prezi também criou regras no AWS Config para gerir o provisionamento e configuração dos seus recursos no AWS. Além disso, a Prezi também usa o AWS CloudTrail para a compliance.

Adicionalmente, a Prezi moveu dois dos seus mais importantes serviços de back-end para o AWS Elastic Beanstalk, que implementa e escala aplicações web e serviços automaticamente. Isto permite aos developers da Prezi não se preocuparem tanto com a gestão da infrasestrutura. A Prezi está também a planear mover o resto da sua infraestrutura para AWS com Elastic Beanstalk. Usando a funcionalidade multicontainer Docker, que é providenciado pelo Amazon EC2 Container Service (Amazon ECS), a Prezi pretende criar uma arquitetura de microsserviços que permita aos seus developers rodar ambientes de desenvolvimento personalizados sem se preocuparem com as complexidades de provisionamento da infraestrutura.

Num futuro próximo, a empresa planeia adicionar AWS Key Management Service (Amazon KMS) para encriptar dados e proteger a segurança das suas chaves (de encriptação). E por fim, continuará a avaliar novos serviços oferecidos pela AWS com o objetivo de substituir muitas das soluções criadas in-house.

**Resultados**<br/>
Ao migrar para AWS, a Prezi obteve uma plataforma altamente escalável e automatizada que está a ajudar a acompanhar o passo da empresa com o seu crescimento acelerado. Além do mais, o ambiente user-friendly dos developers, permitiu-lhes avançar rapidamente em ajustes, aumentando a sua produtividade, ao mesmo tempo que tornam simples a visualização de informação que precisam.

AWS possibilitou também à equipa de desenvolvimento acelerar a criação de produto. Usando APIs da Amazon, os developers da Prezi têm a documentação de que precisam para começar e imensa flexibilidade para personalizar soluções. Ao usarem uma arquitetura de microsserviços em combinação com AWS, os developers podem trabalhar em tarefas isoladas sem a proecupação de duplicarem esforços. Capacidades com estas permitem aos programadores Prezi apresentar novos serviços, às vezes, em apenas 1 ou 2 dias, comparando com as semanas ou meses que os ocupavam no passado, ao terem de trabalhar sobre um enorme código base trabalhado por todos (criando a possibilidade de conflitos).

Talvez mais importante, a AWS ajudou a Prezi a cumprir os seus objetivos de se tornar verdadeiramente uma empresa orientada a dados. Com a ajuda do Amazon Redshift, os dados que eram o domínio apenas dos especialistas da equipa de dados da Prezi, passaram agora a ser acedidos por todos na companhia, permitindo dar resposta muito rapidamente aos trabalhadores. Adicionalmente, os líderes da companhia podem analisar maiores quantidades de dados, usando ferramentas de visualização de dados para monitorizar a performance dos produtos Prezi, enquanto recebem informação detalhada sobre os seus utilizadores.

Maior acesso a dados também permitiu à Prezi reter clientes e identificar novas oportunidades de negócio. Por exemplo, gestores de produto agora compreendem melhor o que utilizadores bem-sucedidos têm em comum. Da mesma forma, as equipas de venda e suporte conseguem agora identificar clientes usando apenas uma pequena percentagem de licenças atribuídas para que possam prestar apoio na escolha adequada. Iniciativas como estas estão a melhorar a satisfação dos clientes e estimular o crescimento da receita a longo prazo.

## Tutorial AWS Elastic Beanstalk 

Para dar uma noção duma situação real de como configurar o serviço AWS Elastic Beanstalk, recorremos a um método passo-a-passo que explicará como ativar uma aplicação web usando esta plataforma. 

**Passo 1:** partindo do princípio que temos conta criada na Amazon AWS, acedemos à página de criação de uma nova aplicação usando o serviço AWS Elastic Beanstalk, como é possível ver na figura abaixo.

![1](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config1.png)


**Passo 2:** definimos o nome para a aplicação que estamos a criar de raíz.

![2](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config2.png)


**Passo 3:** em seguida, escolhemos o tipo de ambiente em que iremos operar, ou seja, entre um "web server" ou um "worker". Seleccionamos neste caso a opção "web server".

![3](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config3.png)


**Passo 4:** ainda sobre o ambiente de desenvolvimento, escolhemos a linguagem de programação que será utilizada na implementação da aplicação. Foi escolhida a linguagem PHP para este caso.

![4](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config4.png)


**Passo 5:** no tipo de ambiente é automaticamente atribuído os serviços load balancing e autoscaling, embora seja possível definir uma única instância, não recorrendo assim a nenhum desses serviços adicionais.

![5](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config5.png)


**Passo 6:** Na "versão da aplicação" a fonte selecionada neste caso foi o "sample application", por neste caso estarmos a criar uma aplicação de raiz. Contudo, neste passo poder-se-ia selecionar uma versão duma aplicação que tivessemos já desenvolvido para correr no ambiente que estamos a definir no AWS.

![6](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config6.png)


**Passo 7:** verificamos de seguida se o URL onde iremos correr o ambiente da aplicação está disponível para podermos executá-la.

![7](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config7.png)


**Passo 8:** poderíamos selecionar recursos adicionais ao nosso ambiente, como por exemplo criar uma instância RDS DB, oferecendo a possibilidade de armazenar e gerir bases de dados relacionados à aplicação. Não foi selecionado, neste caso, nenhum recurso adicional.

![8](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config8.png)


**Passo 9:** relativamente aos detalhes de configuração é onde se escolhe o tipo de instância a criar e onde se pode associar ou criar uma key pair. Neste exemplo, já tinha sido criada uma key pair de acesso ao servidor que vai permitir correr a aplicação.

![9](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config9.png)


**Passo 10:** é possível adicionar tags nesta fase da configuração do ambiente de trabalho. Neste caso, não se definiu nenhuma.

![10](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config10.png)


**Passo 11:** numa fase final de configuração faz-se a verificação de todas as etapas e as seleções feitas antes do ambiente ser lançado.

![11](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config11.png)


**Passo 12:** a partir de agora, temos acesso à visão geral da consola onde podemos verificar o estado (health), gerir e monitorizar o ambiente da aplicação que estamos a testar e a executar.

![12](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config12.png)


**Passo 13:** acedemos ao link de acesso à aplicação, através da consola, com a mensagem de confirmação de que a aplicação AWS Elastic Beanstalk PHP está ativa.

![13](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config13.png)


**Passo 14:** é mostrado neste passo, através da consola Amazon EC2, que temos a instância "Deployment server" a correr, sendo esta instância nos permitirá o desenvolvimento e execução da aplicação.

![14](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config14.png)


**Passo 15:** dentro da instância, e usando a linha de comandos, foi criado um diretório onde irá ser criado o ficheiro "index.php" e depois será aberto usando o software GNU nano.

![15](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config15.png)


**Passo 16:** com recurso ao GNU nano é escrito uma linha de código simples para teste (echo "Hello World!";).

![16](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config16.png)


**Passo 17:** agora é lançado o comando para atualizar e ativar a aplicação.

![18](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config18.png)


**Passo 18:** recebemos mensagem pela linha de comandos de que a atualização do ambiente onde será executada a aplicação aconteceu com sucesso.

![19](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config19.png)


**Passo 19:** ao aceder de novo ao link da aplicação, fazemos "refresh" e confirmamos que está a executar como previsto.

![20](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config20.png)


**Passo 20:** depois de termos executado a aplicação, voltamos à consola da AWS Elastic Beanstalk, verificando no separador de Monitorização, algumas das métricas obtidas com os eventos que decorreram da execução.

![21](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config21.png)


**Passo 21:** no separador de Eventos verificamos, precisamente, todos os passos decorridos desde que lançamos o ambiente para implementação da aplicação.

![22](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config24.png)


**Passo 22:** Por último, no separador de Configuração é possível gerir e alterar todas as características do ambiente lançado inicialmente, desde alteração do tipo de instância, como a ativação/desativação do load balancing e autoscaling.

![23](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config22.png)


## Conclusão
O desenvolvimento deste documento permitiu uma melhor compreensão do ambiente de PaaS (Platform as a Service). Para além da análise dos casos de estudo de outras plataformas, o exemplo do Amazon Elastic Beanstalk permitiu perceber melhor o conceito e a funcionalidade do serviço. <br/> Naturalmente, estes serviços surgem da necessidade de responder a desafios que existem em várias frentes onde atuam as Tecnologias de Informação e, como tal, a análise de exemplos de implementação são uma grande ajuda para entender melhor o assunto. Assim, o caso de estudo da Prezi enquanto aplicação criada e mantida com recurso ao Amazon Elastic Beanstalk, elucida-nos quando às funcionalidades e vantagens deste na gestão dos serviços de infraestruturas da AWS.

## Referências
