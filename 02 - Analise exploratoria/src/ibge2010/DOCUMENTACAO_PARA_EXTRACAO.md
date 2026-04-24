# Objetivo

O objetivo desta documentação é orientar a extração e o tratamento de dados socioeconômicos do censo demográfico de 2010, com foco no indicadores de renda e alfabetização em nível de bairro para o município de Curitiba.

Esses dados serão utilizados para investigar possíveis relações entre fatores socioeconômicos e as ocorrências registradas pela SIGESGUARDA.

---

# Fonte da documentação

As informações utilizadas nesta documentação foram extraídas da documentação oficial do IBGE referente às variáveis do universo do censo demográfico de 2010 por setores censitários. 

Os documentos utilizados estão disponíveis em:

https://www.cidadessustentaveis.org.br/arquivos/SIG/documentacao-sig/IBGE_BR-Setores-Censitarios_Censo%202010_Variaveis-universo.pdf

http://www.repositorio.poli.ufrj.br/monografias/monopoli10026310.pdf

---

# Estrutura dos dados do censo demográfico 2010

os dados do censo demográfico de 2010 podem ser obtidos via FTP do IBGE no diretório:

`/Censos/Censo_Demografico_2010/Resultados_do_Universo/Agregados_por_Setores`

---

# Organização dos arquivos

Os dados do censo de 2010 são disponibilizados separadamente para cada Unidade da Federação (UF). Cada UF possui um conjunto de 18 arquivos, organizados em 10 grupos temáticos.

## Grupos de arquivos

### Básico 

Contém os códigos e nomes das subdivisões geográficas, além das informações básicas do cadastro de áreas.

- Quantidade de arquivos: 1

### Domicílio

Contém informações sobre os moradores, segmentadas por sexo, faixa etária e características dos domicílios.

- Quantidade de arquivos: 2

### Alfabetização

Contém informações sobre alfabetização da população residente, segmentadas por sexo e idade.

- Quantidade de arquivos: 2

### Cor e raça 

Contém informações sobre cor ou raça da população, segmentadas por sexo e idade.

- Quantidade de arquivos: 3

### Parentesco

Contém informações sobre relações de parentesco da população residente.

- Quantidade de arquivos: 4

### Registro civil

Contém informações sobre registro de nascimento da população.

- Quantidade de arquivos: 1

### Entorno

Contém informações relacionadas ao entorno das quadras e faces dos setores censitários.

- Quantidade de arquivos: 5

### Renda 

Contém informações sobre rendimentos dos domicílios, moradores e responsáveis pelo domicílio.

- Quantidade de arquivos: 3

---

# Estrutura do código do setor censitário

O código do setor censitário é composto por 15 digitos, organizados da seguinte forma: 

`UFMMMMMDDSDSSSS`

| Componente | Descrição |
|---|---|
| UF | Unidade da Federação |
| MMMMM | Município |
| DD | Distrito |
| SD | Subdistrito |
| SSSS | Setor censitário |

---

# Estrutura do código do bairro

O código do bairro é composto por 10 dígitos, organizados da seguinte forma:

`UFMMMMMBBB`

| Componente | Descrição |
|---|---|
| UF | Unidade da Federação |
| MMMMM | Município |
| BBB | Bairro |