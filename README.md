Essa é uma documentação que vai apresentar um passo a passo para quem for começar no estudo de container. Alguns dos links vão ser em inglês por a maioria da documentação é em inglês. Sempre que possível vou colocar um link também em português para ser mais acessível.

O primeiro passo é sempre a definição. A RedHat, empresa no setor de computação em nuvem, fez um guia muito interessante com o 101 de container.

https://developers.redhat.com/blog/2018/02/22/container-terminology-practical-introduction/

Não se preocupe por que existe muita informação nesse primeiro documento. O próximo passo é usar de fato usar a ferramenta. 

Container surgiram no kernel do Linux e hoje são muito populares se tornando a forma com que a maioria das novas ferramentas são disponibilizadas. Containers tomaram vantagem por encaixar com a filosofia de microserviços, pois são elementos que provem isolamento e rápido provisionamento.

A "container engine" de fato é o Docker. A forma como imagens são disponibilizadas é parte de uma iniciativa para criar compatibilidade entre diversas "engines" e esse padrão universal é baseado na formatação seguida pelo Docker. Logo, o melhor a se fazer é utilizar Docker e, em caso de necessidade, migrar para outra plataforma.

Da mesma forma que Docker é a engine mais recomendada, Kubernetes é o orchestrador mais utilizado é o mais recomendado. Perceba que Docker e Kubernetes (k8s) não são equivalentes. Docker é uma ferramenta que recebe comandos e cria container. Já o Kubernetes controla poll de computação e é capaz de alocar clusters de containes, recuperar de falhas e lidar com balanceamento de carga e scale in e scale out.

Uma boa documentação para aprender Docker você encontra nesse link: https://docker-curriculum.com

Já a documentação para o Kubernetes indicada é essa: https://kubernetes.io/docs/tutorials/kubernetes-basics/

Agora que entendemos o conceito de Containers, Container Engine (Docker) e Orquestrador de Containers (Kubernetes) vamos dar um passo a frente. 

Containers são ferramentas que se adequam perfeitamente a nuvem. Containers utilizam recursos computacionais e nuvens possuem esses recursos em abundância. Hoje, existem 3 grandes provedoras de computação em nuvem: Amazon AWS, Google Cloud e Windows Azure. 

Dessas, o melhor para começar a desenvolver é o Google Cloud, mas por quê?

Primeiro, o Google é o desenvolvedor do Kubernetes. O Kubernetes nasceu de uma ferramenta que os desenvolvedores da Google criaram para gerenciar os containers da sua infraestrutura: Borg. Desse projeto nasce o Kubernetes que logo depois virou um projeto de código aberto.

Segundo, a Google fornece $300 de utilização por um ano. Essa valor é suficiente para aprender e para o desenvolvimento inicial de um projeto.

Terceiro, a documentação e navegação pela ferramenta do Google é muito mais intuitiva.

Quarto, migrar de uma ferramenta de nuvem para outra não é tão penoso quando se utiliza containers. Dessa forma, é melhor focar no desenvolvimento rápido em, em caso de necessidade, migrar para outra ferramenta.

A primeira experiência com containers em nuvem não pode ser traumática, e por sorte (ou dedicação da comunidade ou vontade de vender mesmo), existe uma aplicação modelo para rodar na Google Kubernetes Engine (o serviço de nuvem voltado para containers). Essa aplicação modelo você encontra nesse link: https://github.com/GoogleCloudPlatform/microservices-demo

Essa aplicação utiliza vários containers rodando aplicações diferentes com linguagens diferentes. Ou seja, um bom exemplo de aplicações reais. Com ela é possível tem um sentimento em relação a ferramentas de deploy em nuvem.

