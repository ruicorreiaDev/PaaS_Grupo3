# **PaaS - Quase Tudo Sobre Amazon Elastic Beanstalk**

# **Resumo**

## **Introdução** <br/> 
![PaaSEstrutura](
Um dos conceitos relacionados com serviços de computação na nuvem é PaaS (Platform as a Service), que normalmente de situa entre o IaaS (Infrastructure as a Service) e o SaaS (Software as a Service). <br/> Podemos definir PaaS como uma categoria de serviços de computação na nuvem que fornece uma plataforma para desenvolver, implementar e executar aplicações, sem o custo e complexidade de implantação e gestão das infraestruturas necessárias. <br/> Para uma melhor compreensão do conceito de PaaS, começamos por apresentar dois casos de estudo, um para a plataforma Heroku e outro para a plataforma Google App Engine. <br/> Posto isto, passamos a apresentar o serviço Elastic Beanstalk, da AWS, que pretendemos conhecer melhor por meio das definições que nos são apresentadas pelo próprio fornecedor ou por terceiros.  

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
