# Features

 - Trocar a biblioteca do mapa, para que adicione o pointer sem precisar das coordenadas 
 - Adicionar banco de dados (supabase) e login ( Cadastrar Pontos de Ajuda, com dados de responsável pelo ponto de apoio para que evite cadastros falsos)
 - Adicionar no formulário de cadastro do ponto de apoio as categorias ( Agua Potável, Alimentos, Abrigo, Saúde, Outros )
 - Adicionar na tela de "Pontos de Apoio" um filtro de busca
 - Melhorar o sobre, utilizar um texto diferente do que está sendo utilizado atualmente e uma interface mais bonita
 

# Engenharia de Requisitos

 - Criar um sistema de validação de cpf para criar pontos de apoio, para evitar cadastros falsos.

 - Criar DB com as tabelas do banco, tabelas de categoria, de pontos de apoio, de usuário. Definir o schema do banco de dados.

 - Criar um sistema de login e senha para que o usuário possa criar pontos de apoio.

 - Cada ponto no mapa, ao clicar deve abrir um card com as informações do ponto de apoio, com as seguintes informações:
    - Nome do ponto de apoio
    - Categoria do ponto de apoio
    - Descrição do ponto de apoio
    - Responsável pelo ponto de apoio
    - Telefone do ponto de apoio
    - Endereço do ponto de apoio
    - Horário de funcionamento
    - Disponibilidade do ponto de apoio
    - Informativo se aceita voluntários 
    - Botão de ir para o local  (Abrir o Waze para traçar a rota)

 - Criar categorias para os pontos de apoio, para que o usuário possa filtrar os pontos de apoio por categoria: 
    - Agua Potável
    - Alimentos
    - Abrigo (Masculino, Feminino, Familiar)
    - Saúde
    - Serviços
    - Doações Roupas
    - Doações Móveis ou Objetos
    - Abrigo de Pets 

 - Criar um sistema de tempo de visibilidade do ponto de apoio embasado nas categorias. Exemplo: 
    - Agua Potável: 5h 
    - Alimentos: 5h 
    - Abrigo: 24h
    - Saúde: 24h
    - Serviços: 5h
    - Doações Roupas: 5h 
    - Doações Móveis ou Objetos: 5hr 
    E após esse período, a visibilidade do abrigo é retirada do mapa, a não ser que o usuário responsável pelo abrigo renova a visibilidade, clicando em um botão de renovar.

# Questões
 - Onde rodar essa aplicação web?
 - Como validar o CPF  -> Fazer login apenas para quem for cadastrar ponto de apoio, ou utilizar outra forma de validação.
 - Como funciona a API que envia a mensagem pelo WhatsApp?  
 - Como proteger os dados sensíveis do usuário?
 - Como adequar o projeto a LGPD?
 - Como o projeto será mantido? 
 - Como guardar os pontos de acesso já criados no mapa  mas tirar a visibilidade deles, para que o criador apenas reative a visibilidade? 


 