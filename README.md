# PaaS_Grupo3

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
