# PaaS_Grupo3

## Caso de Estudo – Prezi 

### Circunstâncias 

Fundada em 2009, Prezi é uma empresa que desenvolve software de apresentações baseado em computação na nuvem. A sua missão é reinventar o método de criar apresentações ao oferecer, aos utilizadores, as ferramentas necessárias para organizar claramente as ideias pretendidas e apresentá-las da forma mais cativante e interativa possível.  

### Desafio 

Para ser capaz de acompanhar o crescimento acentuado, a Prezi precisava de uma plataforma em cloud, com grande capacidade de escalabilidade e automação, que hospedasse o seu software como um serviço. Era crítico, também, que a plataforma fosse flexível, intuitiva e fácil de gerir, para que os developers pudessem rapidamente criar novas funcionalidades para os clientes. Além do mais, a empresa precisava de uma plataforma cloud capaz de oferecer a maior confiabilidade possível, que servisse os mais de 1 milhão de novos clientes que aderem ao Prezi por mês. 
 
Os trabalhadores da Prezi também necessitavam de uma maneira rápida de analisar e visualizar dados para que pudessem melhorar a oferta dos seus serviços. Contudo, quando os trabalhadores precisavam de informação, era-lhes exigido contactar com a equipa de dados, que por sua vez escreviam código específico para cada caso, movendo manualmente os dados para uma tabela de forma a fazer análise. Com tantos pedidos a surgir de diferentes partes da empresa, a equipa de dados normalmente acumulava serviço, demorando por vezes dias a dar resposta. 

### Estratégia (Porquê AWS?) 

Nos primeiros anos de negócio, a Prezi hospedava as suas ferramentas de apresentação interativas numa plataforma gerida em cloud, com muitos dos seus serviços desenvolvidos on-premises. A organização eventualmente começou a migrar os seus SaaS para a Amazon Web Services (AWS) em 2012 por causa da alta escalabilidade da plataforma. 

A Prezi foi também atraída pela AWS por causa do serviço Amazon Redshift, uma solução de armazenamento de dados que permite a análise de uma forma simples e com elevado custo-benefício. A empresa pretendia que todos os empregados fossem capazes de aceder a dados sem terem de esperar pela ajuda da equipa especializada em dados. Além do mais a Prezi queria tornar simples o processo de visualização de dados para que fosse possível, rapidamente, detetar tendências e ajustar os seus produtos com base no que é procurado pelos clientes. 

Além do Redshift, a Prezi depende de outros componentes de base de dados AWS incluindo Amazon Relational Database Service (Amazon RDS) para operar e escalar o servidor SQL na cloud; Amazon DynamoDB, para armazenar metadados e mover dados entre aplicações; Amazon ElastiCache para implementar, operar e escalar uma in-memory cache na cloud; e Amazon Simple Storage Service (Amazon S3) para armazenar apresentações de utilizadores e servir de back up para as outras bases de dados da empresa. 

Para análise, a Prezi utiliza Amazon Elastic MapReduce (Amazon EMR), que permite aos developers processar de forma simples e eficiente grandes quantidades de dados. Para computação, a organização usa instâncias da Amazon Elastic Compute Cloud (Amazon EC2).  A Prezi depende de AWS Config para segurança e gestão. Esse serviço rastreia as alterações de configuração aos recursos do Prezi no AWS e envia notificações sempre que os recursos são criados, alterados ou apagados. A Prezi também criou regras no AWS Config para gerir o provisionamento e configuração dos seus recursos no AWS. Além disso, a Prezi também usa o AWS CloudTrail para a compliance. 

 
Adicionalmente, a Prezi moveu dois dos seus mais importantes serviços de back-end para o AWS Elastic Beanstalk, que implementa e escala aplicações web e serviços automaticamente. Isto permite aos developers da Prezi não se preocuparem tanto com a gestão da infrasestrutura. A Prezi está também a planear mover o resto da sua infraestrutura para AWS com Elastic Beanstalk. Usando a funcionalidade multicontainer Docker, que é providenciado pelo Amazon EC2 Container Service (Amazon ECS), a Prezi pretende criar uma arquitetura de microsserviços que permita aos seus developers rodar ambientes de desenvolvimento personalizados sem se preocuparem com as complexidades de provisionamento da infraestrutura. 

Num futuro próximo, a empresa planeia adicionar AWS Key Management Service (Amazon KMS) para encriptar dados e proteger a segurança das suas chaves (de encriptação). E por fim, continuará a avaliar novos serviços oferecidos pela AWS com o objetivo de substituir muitas das soluções criadas in-house. 

### Resultados 

Ao migrar para AWS, a Prezi obteve uma plataforma altamente escalável e automatizada que está a ajudar a acompanhar o passo da empresa com o seu crescimento acelerado. Além do mais, o ambiente user-friendly dos developers, permitiu-lhes avançar rapidamente em ajustes, aumentando a sua produtividade, ao mesmo tempo que tornam simples a visualização de informação que precisam. 

AWS possibilitou também à equipa de desenvolvimento acelerar a criação de produto. Usando APIs da Amazon, os developers da Prezi têm a documentação de que precisam para começar e imensa flexibilidade para personalizar soluções. Ao usarem uma arquitetura de microsserviços em combinação com AWS, os developers podem trabalhar em tarefas isoladas sem a proecupação de duplicarem esforços. Capacidades com estas permitem aos programadores Prezi apresentar novos serviços, às vezes, em apenas 1 ou 2 dias, comparando com as semanas ou meses que os ocupavam no passado, ao terem de trabalhar sobre um enorme código base trabalhado por todos (criando a possibilidade de conflitos). 
 
Talvez mais importante, a AWS ajudou a Prezi a cumprir os seus objetivos de se tornar verdadeiramente uma empresa orientada a dados. Com a ajuda do Amazon Redshift, os dados que eram o domínio apenas dos especialistas da equipa de dados da Prezi, passaram agora a ser acedidos por todos na companhia, permitindo dar resposta muito rapidamente aos trabalhadores. Adicionalmente, os líderes da companhia podem analisar maiores quantidades de dados, usando ferramentas de visualização de dados para monitorizar a performance dos produtos Prezi, enquanto recebem informação detalhada sobre os seus utilizadores. 
 

Maior acesso a dados também permitiu à Prezi reter clientes e identificar novas oportunidades de negócio. Por exemplo, gestores de produto agora compreendem melhor o que utilizadores bem-sucedidos têm em comum. Da mesma forma, as equipas de venda e suporte conseguem agora identificar clientes usando apenas uma pequena percentagem de licenças atribuídas para que possam prestar apoio na escolha adequada. Iniciativas como estas estão a melhorar a satisfação dos clientes e estimular o crescimento da receita a longo prazo. 


## Guia Passo a Passo 

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

![24](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config23.png)
