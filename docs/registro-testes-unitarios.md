# Registro de Testes de Endpoint
Aluno: Isabela # Registro de Testes de Endpoint
Aluno: Isabela Viana
Grupo: Grupo 02
## Testes escritos
| # | Verbo e rota | Com token? | Status esperado | Verde ou vermelho? |
| --- | ------------ | ---------- | --------------- | ------------------ |
| 1 | POST /eventos | Sim | 201 | Verde |
| 2 | GET /eventos/:id | Não | 404 | Verde |
| 3 | GET /eventos/:id | Não | 400 | Vermelho |
## Resultado
Linha "Tests:" da saída do npm run test:endpoint: Tests: 1 failed, 4 passed, 5 total
## Defeito encontrado
Teste: GET /eventos/:id (rota pública) › responde 400 quando o id tem letras
Esperado: Status 400 (erro de requisição inválida, pois o ID contém letras)
Obtido: Status 200 (a API aceitou o ID com letras e retornou o evento cadastrado)
Em qual aula esse mesmo defeito já tinha aparecido, e como: Na Aula 04 (testes unitários), na função parseId("12abc"), que usava parseInt e extraía apenas os números iniciais (12), ignorando as letras no final em vez de rejeitar a entrada.
Grupo: Nome/Número do Grupo
## Testes escritos
| # | Verbo e rota | Com token? | Status esperado | Verde ou vermelho? |
| --- | ------------ | ---------- | --------------- | ------------------ |
| 1 | POST /eventos | Sim | 201 | Verde |
| 2 | GET /eventos/:id | Não | 404 | Verde |
| 3 | GET /eventos/:id | Não | 400 | Vermelho |
## Resultado
Linha "Tests:" da saída do npm run test:endpoint: Tests: 1 failed, 4 passed, 5 total
## Defeito encontrado
Teste: GET /eventos/:id (rota pública) › responde 400 quando o id tem letras
Esperado: Status 400 (erro de requisição inválida, pois o ID contém letras)
Obtido: Status 200 (a API aceitou o ID com letras e retornou o evento cadastrado)
Em qual aula esse mesmo defeito já tinha aparecido, e como: Na Aula 04 (testes unitários), na função parseId("12abc"), que usava parseInt e extraía apenas os números iniciais (12), ignorando as letras no final em vez de rejeitar a entrada.