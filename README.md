# laboratorio_clinico
🧪 Laboratório Clínico – Sistema de Processamento de Exames

Este repositório contém um projeto acadêmico que simula o funcionamento básico de um sistema de gerenciamento de exames em um laboratório clínico, desenvolvido em Portugol.
O objetivo é demonstrar a lógica aplicada em rotinas de cadastro de pacientes, registro de exames, cálculos simples e emissão de resultados.

Var
// Seção de Declarações das variáveis 
 login, senha, nomePaciente, cpf: caractere
   nomeExame, statusExame: caractere
   usuarioAutenticado: logico
   preco: real

Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 

   escreval("--- 1. ACESSO AO SISTEMA ---")
   escreva("Login de Funcionário: ")
   leia(login)
   escreva("Senha: ")
   leia(senha)

   se (login = "lab" ) e (senha = "123") entao
      usuarioAutenticado <- verdadeiro
      escreval("Acesso liberado!")
   senao
      usuarioAutenticado <- falso
      escreval("Acesso negado.")
   fimse
   escreval


   escreval("--- 2. CADASTRO DE PACIENTE ---")
   escreva("Nome do Paciente: ")
   leia(nomePaciente)
   escreva("CPF do Paciente: ")
   leia(cpf)
   escreval("Paciente ", nomePaciente, " (CPF: ", cpf, ") cadastrado com sucesso.")
   escreval


   escreval("--- 3. REGISTRO DE EXAME ---")
   escreva("Nome do Exame: ")
   leia(nomeExame)
   escreva("Preço do Exame: R$ ")
   leia(preco)

   statusExame <- "Aguardando Coleta" // Status inicial
   escreval("Exame ", nomeExame, " (R$ ", preco:2:2, ") solicitado.")
   escreval("Status: ", statusExame)

   // Simulação de Emissão de Resultado (Atualização de Status)
   statusExame <- "Laudo Disponível"
   escreval("-> [AÇÃO DO SISTEMA] Novo Status (Resultado Pronto): ", statusExame)

Fimalgoritmo
