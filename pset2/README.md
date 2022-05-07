# - Pset2 -
### Aprendendo a desenvolver relatórios em linguagem SQL

>[!NOTE]
>
> Todos os relatórios foram feitos em cima do projeto lógico implementado no [_Pset1_](https://github.com/JoaoLucasAssis/uvv_bd_1_cc1m/blob/main/pset1).

---

[01](#questão_01) • 
[02](#questão_02) • 
[03](#questão_03) • 
[04](#questão_04) • 
[05](#questão_05) • 
[06](#questão_06) • 
[07](#questão_07) • 
[08](#questão_08) •
[09](#questão_09) •
[10](#questão_10) •
[11](#questão_11) •
[12](#questão_12) •
[13](#questão_13) •
[14](#questão_14) •
[15](#questão_15)

## QUESTÃO_01: 

Relatório que mostra a média salarial dos funcionários de cada departamento.

| numero_departamento | media_salario |
|---------------------|---------------|
|                   1 |      55000.00 |
|                   4 |      31000.00 |
|                   5 |      33250.00 |

## QUESTÃO_02:

Relatório que mostra a média salarial dos homens e das mulheres.

| sexo | media_salario |
|------|---------------|
| M    |      37600.00 |
| F    |      31000.00 |

## QUESTÃO_03:

Relatório que lista o nome dos departamentos e, para cada departamento, o nome completo, 
a data de nascimento, a idade em anos completos e o salário dos funcionários.

| nome_departamento | nome_funcionario | data_nascimento | idade_funcionario | salario  |
|-------------------|------------------|-----------------|-------------------|----------|
| Matriz            | Jorge E Brito    | 1937-11-10      |                84 | 55000.00 |
| Administração     | Jennifer S Souza | 1941-06-20      |                80 | 43000.00 |
| Administração     | André V Pereira  | 1969-03-29      |                53 | 25000.00 |
| Administração     | Alice J Zelaya   | 1968-01-19      |                54 | 25000.00 |
| Pesquisa          | João B Silva     | 1965-01-09      |                57 | 30000.00 |
| Pesquisa          | Fernando T Wong  | 1955-12-08      |                66 | 40000.00 |
| Pesquisa          | Joice A Leite    | 1972-07-31      |                49 | 25000.00 |
| Pesquisa          | Ronaldo K Lima   | 1962-09-15      |                59 | 38000.00 |

## QUESTÃO_04:

Relatório que mostra o nome completo dos funcionários, a idade em anos completos, o salário atual e o salário reajustado.

| nome_funcionario | idade_funcionario | salario_atual | salario_reajuste |
|------------------|-------------------|---------------|------------------|
| João B Silva     |                57 |      30000.00 |         36000.00 |
| Fernando T Wong  |                66 |      40000.00 |         46000.00 |
| Joice A Leite    |                49 |      25000.00 |         30000.00 |
| Ronaldo K Lima   |                59 |      38000.00 |         43700.00 |
| Jorge E Brito    |                84 |      55000.00 |         63250.00 |
| Jennifer S Souza |                80 |      43000.00 |         49450.00 |
| André V Pereira  |                53 |      25000.00 |         30000.00 |
| Alice J Zelaya   |                54 |      25000.00 |         30000.00 |

## QUESTÃO_05:

Relatório que lista, para cada departamento, o nome do gerente e o nome dos funcionários.

| nome_departamento | nome_gerente     | nome_funcionario | salario  |
|-------------------|------------------|------------------|----------|
| Administração     | Jennifer S Souza | Jennifer S Souza | 43000.00 |
| Administração     | Jennifer S Souza | André V Pereira  | 25000.00 |
| Administração     | Jennifer S Souza | Alice J Zelaya   | 25000.00 |
| Matriz            | Jorge E Brito    | Jorge E Brito    | 55000.00 |
| Pesquisa          | Fernando T Wong  | Fernando T Wong  | 40000.00 |
| Pesquisa          | Fernando T Wong  | Ronaldo K Lima   | 38000.00 |
| Pesquisa          | Fernando T Wong  | João B Silva     | 30000.00 |
| Pesquisa          | Fernando T Wong  | Joice A Leite    | 25000.00 |

## QUESTÃO_06:

Relatório que mostra o nome completo dos funcionários que têm dependentes, o departamento onde eles trabalham e, para cada funcionário, o nome completo dos dependentes, a idade em anos de cada dependente e o sexo.

| nome_funcionario | numero_departamento | nome_dependente | idade_dependente | sexo_dependente |
|------------------|---------------------|-----------------|------------------|-----------------|
| João B Silva     |                   5 | Alícia          |               33 | feminino        |
| João B Silva     |                   5 | Elizabeth       |               55 | feminino        |
| João B Silva     |                   5 | Michael         |               34 | masculino       |
| Fernando T Wong  |                   5 | Alícia          |               36 | feminino        |
| Fernando T Wong  |                   5 | Janaína         |               64 | feminino        |
| Fernando T Wong  |                   5 | Tiago           |               38 | masculino       |
| Jennifer S Souza |                   4 | Antonio         |               80 | masculino       |

## QUESTÃO_07:

Relatório que mostra, para cada funcionário que não tem dependente, seu nome completo, departamento e salário.

| nome_funcionario | nome_departamento | salario  |
|------------------|-------------------|----------|
| Jorge E Brito    | Matriz            | 55000.00 |
| André V Pereira  | Administração     | 25000.00 |
| Alice J Zelaya   | Administração     | 25000.00 |
| Joice A Leite    | Pesquisa          | 25000.00 |
| Ronaldo K Lima   | Pesquisa          | 38000.00 |

## QUESTÃO_08:

Relatório que mostra, para cada departamento, os projetos desse departamento e o nome completo dos funcionários que estão alocados
em cada projeto. E em cada projeto, o número de horas trabalhadas por cada funcionário.

| nome_departamento | nome_funcionario | nome_projeto    | horas |
|-------------------|------------------|-----------------|-------|
| Matriz            | Jorge E Brito    | Reorganização   |   0.0 |
| Administração     | Jennifer S Souza | Reorganização   |  15.0 |
| Administração     | Jennifer S Souza | Novosbenefícios |  20.0 |
| Administração     | André V Pereira  | Informatização  |  35.0 |
| Administração     | André V Pereira  | Novosbenefícios |   5.0 |
| Administração     | Alice J Zelaya   | Informatização  |  10.0 |
| Administração     | Alice J Zelaya   | Novosbenefícios |  30.0 |
| Pesquisa          | João B Silva     | ProdutoX        |  32.5 |
| Pesquisa          | João B Silva     | ProdutoY        |   7.5 |
| Pesquisa          | Fernando T Wong  | ProdutoY        |  10.0 |
| Pesquisa          | Fernando T Wong  | ProdutoZ        |  10.0 |
| Pesquisa          | Fernando T Wong  | Informatização  |  10.0 |
| Pesquisa          | Fernando T Wong  | Reorganização   |  10.0 |
| Pesquisa          | Joice A Leite    | ProdutoX        |  20.0 |
| Pesquisa          | Joice A Leite    | ProdutoY        |  20.0 |
| Pesquisa          | Ronaldo K Lima   | ProdutoZ        |  40.0 |

## QUESTÃO_09:

Relatório que mostra a soma total das horas de cada projeto em cada departamento.

| nome_departamento | nome_projeto    | horas_trabalhadas |
|-------------------|-----------------|-------------------|
| Administração     | Informatização  |              55.0 |
| Administração     | Novosbenefícios |              55.0 |
| Matriz            | Reorganização   |              25.0 |
| Pesquisa          | ProdutoX        |              52.5 |
| Pesquisa          | ProdutoY        |              37.5 |
| Pesquisa          | ProdutoZ        |              50.0 |

## QUESTÃO_10:

Relatório que mostre a média salarial dos funcionários de cada departamento.

| departamento | media_salário |
|--------------|---------------|
|            1 |      55000.00 |
|            4 |      31000.00 |
|            5 |      33250.00 |

## QUESTÃO_11:

Relatório que mostra o nome completo do funcionário, o nome do projeto e o valor total que o funcionário receberá referente às horas trabalhadas naquele projeto.

| nome_funcionario | numero_projeto | horas_trabalhadas | total_pago |
|------------------|----------------|-------------------|------------|
| João B Silva     |              1 |              32.5 |     1625.0 |
| Joice A Leite    |              1 |              20.0 |     1000.0 |
| Joice A Leite    |              2 |              20.0 |     1000.0 |
| Fernando T Wong  |              2 |              10.0 |      500.0 |
| João B Silva     |              2 |               7.5 |      375.0 |
| Ronaldo K Lima   |              3 |              40.0 |     2000.0 |
| Fernando T Wong  |              3 |              10.0 |      500.0 |
| André V Pereira  |             10 |              35.0 |     1750.0 |
| Fernando T Wong  |             10 |              10.0 |      500.0 |
| Alice J Zelaya   |             10 |              10.0 |      500.0 |
| Jennifer S Souza |             20 |              15.0 |      750.0 |
| Fernando T Wong  |             20 |              10.0 |      500.0 |
| Jorge E Brito    |             20 |               0.0 |        0.0 |
| Alice J Zelaya   |             30 |              30.0 |     1500.0 |
| Jennifer S Souza |             30 |              20.0 |     1000.0 |
| André V Pereira  |             30 |               5.0 |      250.0 |

## QUESTÃO_12:

Relatório que lista o nome do departamento, o nome do projeto e o nome dos funcionários que, mesmo estando alocados a algum projeto, não registraram nenhuma hora trabalhada.

| nome_departamento | nome_projeto  | nome_funcionario |
|-------------------|---------------|------------------|
| Matriz            | Reorganização | Jorge E Brito    |

## QUESTÃO_13:

Relatório que lista o nome completo dos funcionários e dependentes, o sexo e a idade em anos completos.

| nome_funcionario | sexo_funcionario | idade |
|------------------|------------------|-------|
| Jorge E Brito    | M                |    84 |
| Jennifer S Souza | F                |    80 |
| Antonio          | M                |    80 |
| Fernando T Wong  | M                |    66 |
| Janaína          | F                |    64 |
| Ronaldo K Lima   | M                |    59 |
| João B Silva     | M                |    57 |
| Elizabeth        | F                |    55 |
| Alice J Zelaya   | F                |    54 |
| André V Pereira  | M                |    53 |
| Joice A Leite    | F                |    49 |
| Tiago            | M                |    38 |
| Alícia           | F                |    36 |
| Michael          | M                |    34 |
| Alícia           | F                |    33 |

## QUESTÃO_14:

Relatório que exibe quantos funcionários cada departamento tem.

| numero_departamento | qtd_funcionario |
|---------------------|-----------------|
|                   1 |               1 |
|                   4 |               3 |
|                   5 |               4 |

## QUESTÃO_15:

Relatório que exibe o nome completo do funcionário, o departamento desse funcionário e o nome dos projetos em que cada funcionário está alocado.

| nome_funcionario | numero_departamento | nome_projeto    |
|------------------|---------------------|-----------------|
| João B Silva     |                   5 | ProdutoX        |
| João B Silva     |                   5 | ProdutoY        |
| Fernando T Wong  |                   5 | Informatização  |
| Fernando T Wong  |                   5 | ProdutoY        |
| Fernando T Wong  |                   5 | ProdutoZ        |
| Fernando T Wong  |                   5 | Reorganização   |
| Joice A Leite    |                   5 | ProdutoX        |
| Joice A Leite    |                   5 | ProdutoY        |
| Ronaldo K Lima   |                   5 | ProdutoZ        |
| Jorge E Brito    |                   1 | Reorganização   |
| Jennifer S Souza |                   4 | Novosbenefícios |
| Jennifer S Souza |                   4 | Reorganização   |
| André V Pereira  |                   4 | Informatização  |
| André V Pereira  |                   4 | Novosbenefícios |
| Alice J Zelaya   |                   4 | Informatização  |
| Alice J Zelaya   |                   4 | Novosbenefícios |















