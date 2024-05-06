# ponderada_m6_s3_banco

# Introdução
&emsp;Esta entrega consiste na conclusão da atividade de desenvolvimento de um banco de dados para aprimorar a prestação de serviços de transporte relacionados à saúde e à entrega de produtos médicos. 

## 1. Modelo Lógico do Banco de Dados
&emsp;O modelo lógico foi criado para atender minimamente ao problema proposto, considerando as entidades Paciente, Veiculo, ProdutoMédico, UnidadeSaude, Transporte e Entrega. O diagrama do modelo lógico pode ser visualizado a seguir:

(imagem diagrama)

### Relacionamentos das tabelas:

**De Paciente para Unidade de Saúde**: Essa relação é de 1 para N, pois um paciente está associado a uma única unidade de saúde, mas uma unidade de saúde pode estar associada a vários pacientes.

**De Paciente para Produto Médico**: Essa relação é de N para N, pois um paciente pode estar associado a vários produtos médicos, e um produto médico pode estar associado a vários pacientes.

**De Entrega para Unidade de Saúde**: Essa relação é de 1 para N, pois uma entrega é feita para uma única unidade de saúde, mas uma unidade de saúde pode receber várias entregas.

**De Transporte para Unidade de Saúde**: Essa relação é de 1 para N, pois uma unidade de sáude pode ter o registro de vários transportes de pacientes.

**De Entrega para Unidade de Saúde**: Essa relação é de 1 para N, pois uma unidade de sáude pode ter o registro de várias entregas de produtos.

**De Entrega para Produto Médico**: Essa relação é de N para N, pois uma entrega inclui vários produtos médicos, que podem ser entregues várias vezes.

**De Entrega para Veículo**: Essa relação é de N para 1, pois uma entrega é realizada por um único veículo, mas um veículo pode realizar várias entregas.

**De Transporte para Veículo**: Essa relação é de 1 para 1, pois um veículo só pode transportar um paciente por vez.

## 2. Deploy do Banco de Dados no MySQL RDS da AWS
&emsp;O banco de dados foi implantado em um serviço MySQL RDS da AWS.

###Passo a passo realizado:
- Criar uma instância RDS utilizando o laboratório do AWS Academy;
- Realizar o deploy do MySQL na instância RDS criada;
- Utilizar o diagrama criado para estruturação do banco
  
