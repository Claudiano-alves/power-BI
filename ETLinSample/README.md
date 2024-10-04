## Mesclagem de Tabelas

A mescla da tabela Funcionários com a tabela Departamentos é realizada pelo seguinte código SQL, gerado no MySQL e extraído para o Power Query:

```sql
CREATE TABLE Employee_Department AS
SELECT 
    e.*,
    d.Dname AS Department_Name,
    d.Mgr_ssn AS Manager_SSN
FROM 
    employee e
INNER JOIN 
    departament d ON e.Dno = d.Dnumber;
```

Mescla das colunas Nome, Nome do meio, e sobrenome usando "Mesclar colunas, com espaço como separador".

### Mesclagem vs. Atribuição Direta

- **Mesclagem**: A mescla (join) é necessária quando você quer combinar dados de duas tabelas diferentes com base em um campo comum (neste caso, o CPF do gerente). Ela permite trazer colunas de uma tabela para outra com base nessa chave, como trazer o nome do gerente da tabela **Funcionários** para a tabela **Departamentos** usando o CPF como referência.

- **Atribuição direta**: A atribuição direta seria utilizada apenas se estivéssemos tentando modificar valores dentro de uma única tabela. Como estamos lidando com duas tabelas distintas e precisamos de dados de ambas, a mescla é o caminho correto. Uma atribuição só funcionaria se a coluna de nome do gerente já estivesse presente na tabela de **Departamentos**, o que não é o caso aqui.

Dados de quantidade de colaboradores por Gerente foram realizados através da mescla das colunas:

- `table.Departamento[CPF do Gerente do Departamento]`
- `table.Funcionários[CPF]`
