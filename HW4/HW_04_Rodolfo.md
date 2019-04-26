Consumer Driven Contracts, segundo Martin Fowler (1) , são uma abordagem na qual o serviço provedor incorpora os consumer contracts, ou seja, as expectativas que o serviços consumidores tem sobre a funcionalidades que devem ser expostas pelo provedor. É uma forma dos serviços consumidores informar ao serviço provedor quais suas expectativas referentes as funcionalidades necessárias.
Isto garante que o provedor esteja ciente de quais funcionalidades são usadas pelos consumidores e qual impacto uma mudança no provedor gera no conjunto de serviços consumidores. 
Ainda segundo Martin Fowler, os CDCs tem as seguintes caracerísticas:
Fechado e completo; Singular e não autoritativos e estável.
Os CDCs se relacionam com microserviços pois existe um conjunto de serviços que precisam interagir para que o sistema funcione. Assim, como CDCs permitem que saibamos quais os impactos da evolução de um serviço no conjunto de serviços que se realacionam com ele.  

Postew's Law também se relaciona com CDC's pois como um serviço provedor geralmente atente as expectativas de um conjunto de serviços consumidores, eventualmente um consumidor pode receber mais informação do que necessita( informações que atente outros consumidores). Isto não deve fazer o consumidor quebrar. Logo o consumidor deve ser aberto no que recebe, verificando apenas se existe o mínimo de informações necessárias para que possa operar.

What are the main solutions (patterns, architectural styles, tools, etc.) to implement:

Message-oriented services - RabbitMQ por exemplo
HTTP and REST endpoints - Spring Boot,
Optimized communication protocols - HATEOAS
API documentations - SWAGGER


4.3. Microservices challenges - Data islands
How can be done data porting from microservices to a data lake or a data warehouse? Explain in details your answer.

Idealmente, um microserviços deve ter todos os dados necessários dentro de si. Assim, evita-se um forte acoplamento entre microserviços, o que dificultaria a evolução dos mesmos, além de dificultar a escalabilidade, pois tem-se a necessidade de sincronizar os dados entre microserviços.







