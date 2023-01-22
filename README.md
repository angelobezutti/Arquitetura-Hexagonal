# Arquitetura Hexagonal
Também conhecida como "Ports and Adapters", a arquitetura hexagonal é um padrão para desenvolvimento de softwares.

A idéia da arquitetura hexagonal é podermos isolar toda a nossa regra de negócio, a camada de dominio e lógica do mundo externo através de portas e adaptadores.

# Imagens Ilustrativas
<div style="display: inline_block" align="center"><br>
  <img align="center" alt="Angelo-java" height="200" width="300" src="https://paulovich.net/static/hexagonal-1.png">
  <img align="center" alt="Angelo-java" height="200" width="300" src="https://miro.medium.com/max/1400/1*yR4C1B-YfMh5zqpbHzTyag.png">
  <img align="center" alt="Angelo-java" height="200" width="300" src="https://static.packt-cdn.com/products/9781839211966/graphics/B15547_02_04.jpg">
</div>

# Application
### &nbsp; **Core**: 
&emsp; &emsp; Onde ficam as regras de negócio e não dever ter acesso direto ao mundo exterior
#### &emsp; Domain:
&emsp; &emsp; Classes de modelo
#### &emsp; Usecase:
&emsp; &emsp; Regras de negócio
### &nbsp; **Ports**: 
&emsp; &emsp; Entradas e saidas
#### &emsp; In: 
&emsp; &emsp; Portas de entrada para o core
#### &emsp; Out:
&emsp; &emsp; Portas de saida do core

# Adapters
### &nbsp; In: 
&emsp; &emsp; Entrada para a aplicação
#### &emsp; Controller: 
&emsp; &emsp; Controlladores
#### &emsp; Consumer: 
&emsp; &emsp; Consumidores
### &nbsp; Out: 
&emsp; &emsp; Saída da aplicação (base de dados, Microserviços)
#### &emsp; Client: 
&emsp; &emsp; Client para acessar outros Microserviços
#### &emsp; Repository: 
&emsp; &emsp; Acesso ao banco de dados

# Config
Configurações da aplicação
