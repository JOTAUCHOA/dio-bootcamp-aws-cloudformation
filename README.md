# dio-bootcamp-aws-cloudformation
Desafio 2 do bootcamp da DIO sobre Cloudformation

# O projeto tem a premissa de ser utilizado para um sistema interno.

# Este projeto funciona da seguinte forma. Composição de elementos:
- 2 Máquinas virtuais
- 2 Elactic Load Balancer
- 1 S3 bucket 
- 1 Role contendo a permissão de acesso ao bucket
- 1 Perfil de acesso atrelado a role de permissão
- 1 subnet
- 1 VPC

# Propósito de cada elemento:

- S3 bucket: Hospedagem de recursos, que podem ser os arquivos de visualização.
- Máquinas virtuais: tem acesso aos arquivos do S3 para disponibilizar aos usuários.
- Roles: Possui a permissões de acesso ao bucket.
- Perfils: Estão atrelados as roles, e estão atribuindos as máquinas virtuais, que dão acesso ao bucket.
- Subnet: Comunição de entre as maquinas virtuais dentro de mesmas rede.
- VPC: Rede virtual comum para máquinas virtuais.
- Elastic Load: Controle de carga de acesso para as máquinas e a para vpc

  
