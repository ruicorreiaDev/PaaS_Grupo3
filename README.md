# PaaS_Grupo3

Para dar uma noção duma situação real de como configurar o serviço AWS Elastic Beanstalk, recorremos a um método passo-a-passo que explicará como ativar uma aplicação web usando esta plataforma. 

Passo 1: partindo do princípio que temos conta criada na Amazon AWS, acedemos à página de criação de uma nova aplicação usando o serviço AWS Elastic Beanstalk, como é possível ver na figura abaixo.

![1](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config1.png)


Passo 2: definimos o nome para a aplicação que estamos a criar de raíz.

![2](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config2.png)


Passo 3: seguidamente, escolhemos o tipo de ambiente em que iremos operar, ou seja, entre um "web server" ou um "worker". Seleccionamos neste caso a opção "web server".

![3](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config3.png)


Passo 4: ainda sobre o ambiente de desenvolvimento, escolhemos a linguagem de programação que será utilizada na implementação da aplicação. Foi escolhida a linguagem PHP para este caso.

![4](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config4.png)


Passo 5: no tipo de ambiente é automaticamente atribuído os serviços load balancing e autoscaling, embora seja possível definir uma única instância, não recorrendo assim a nenhum desses serviços adicionais.

![5](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config5.png)


Passo 6: Na "versão da aplicação" a fonte selecionada neste caso foi o "sample application", por neste caso estarmos a criar uma aplicação de raiz. Contudo, neste passo poder-se-ia selecionar uma versão duma aplicação que tivessemos já desenvolvido para correr no ambiente que estamos a definir no AWS.

![6](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config6.png)


Passo 7: verificamos de seguida se o URL onde iremos correr o ambiente da aplicação está disponível para podermos executá-la.

![7](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config7.png)


Passo 8: poderíamos selecionar recursos adicionais ao nosso ambiente, como por exemplo criar uma instância RDS DB, oferecendo a possibilidade de armazenar e gerir bases de dados relacionados à aplicação. Não foi selecionado, neste caso, nenhum recurso adicional.

![8](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config8.png)


Passo 9: relativamente aos detalhes de configuração é onde se escolhe o tipo de instância a criar e onde se pode associar ou criar uma key pair. Neste exemplo, já tinha sido criada uma key pair de acesso ao servidor que vai permitir correr a aplicação.

![9](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config9.png)

![10](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config10.png)

![11](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config11.png)

![12](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config12.png)

![13](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config13.png)

![14](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config14.png)

![15](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config15.png)

![16](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config16.png)

![17](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config17.png)

![18](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config18.png)

![19](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config19.png)

![20](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config20.png)

![21](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config21.png)

![22](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config22.png)

![23](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config23.png)

![24](https://github.com/ruicorreiaDev/PaaS_Grupo3/blob/main/Configura%C3%A7%C3%A3o%20AWS%20Elastic%20Beanstalk/config24.png)
