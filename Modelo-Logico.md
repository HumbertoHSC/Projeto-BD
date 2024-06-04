### Usuário(CPF, nome)
  
- Telefone(CPF, telefone)
  - CPF => Usuario(CPF)

- Endereço(CPF, cep, rua, complemento, bairro)
  - CPF => Usuario(CPF)

- Cliente(CPF)
  - CPF => Usuario(CPF)

- Funcionario(CPF,CHEFE)
  - CHEFE => FUNCIONÁRIO(CPF)


### Veículo(Placa, marca, modelo, cor)


### Possui (CPF, Placa) (Chave primária composta)
-  CPF => Usuario(CPF)
-  Placa => Veículo(Placa)


### Vaga(ID, IdEstacionamento) (Chave primária composta)
-  IdEstacionamento => Estacionamento(ID)


### Reserva(CpfUsuario, Placa, IdVaga, horário, ID_cupom)
-  CpfUsuario => Usuario(CPF)
-  Placa => Veículo(Placa)
-  IdVaga => Vaga(ID)
-  ID_cupom => cupom(ID)


### Estacionamento(ID, taxa, endereço, capacidade,[CPF_funcionário]!) 


### Cupom(ID, valor)

