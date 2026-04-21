## Tabela de dicionário de dados de dados

| COLUNAS|	TIPO |	TAMANHO |	NULL ou NOT NULL |	DESCRIÇÃO DOS CAMPOS|
|--------|------|----------|--------------------|-------------------------|
| ATENDIMENTO_ANO|	int|	-|  NOT NULL|	Ano em que foi realizado o atendimento|
| ATENDIMENTO_BAIRRO_NOME|	varchar|	20|	NOT NULL|	Nome do bairro em que foi realizado o atendimento|
| EQUIPAMENTO_URBANO_NOME|	varchar|	70|	NULL|	Nome do equipamento urbano|
| FLAG_EQUIPAMENTO_URBANO|   	char|	3|	NOT NULL|	Flag para identificar se é um equipamento urbano ou não|
| FLAG_FLAGRANTE| char|	3|	NOT NULL|	Flag para identificar se é um equipamento urbano ou não|
| LOGRADOURO_NOME|	varchar|	70|	NOT NULL|	Nome do logradouro|
| NATUREZA1_DEFESA_CIVIL|	bit|	11|	NULL|	Flag para identificar se é uma natureza de defesa civil ou não (0 - Não, 1 - Sim)|
| NATUREZA1_DESCRICAO|	varchar|	100|	NULL|	Descrição da primeira natureza cadastrada na ocorrência|
| NATUREZA2_DEFESA_CIVIL|	bit|	11|	NULL|	Flag para identificar se é uma natureza de defesa civil ou não (0 - Não, 1 - Sim)|
| NATUREZA2_DESCRICAO|	varchar|	100|	NULL|	Descrição da segunda natureza cadastrada na ocorrência|
| NATUREZA3_DEFESA_CIVIL|	bit|	11|	NULL|	Flag para identificar se é uma natureza de defesa civil ou não (0 - Não, 1 - Sim)|
| NATUREZA3_DESCRICAO|	varchar|	100|	NULL|	Descrição da terceira natureza cadastrada na ocorrência|
| NATUREZA4_DEFESA_CIVIL|	bit|	11|	NULL|	Flag para identificar se é uma natureza de defesa civil ou não (0 - Não, 1 - Sim)|
| NATUREZA4_DESCRICAO|	varchar|	100|	NULL|	Descrição da quarta natureza cadastrada na ocorrência|
| NATUREZA5_DEFESA_CIVIL|	bit|	11|	NULL|	Flag para identificar se é uma natureza de defesa civil ou não (0 - Não, 1 - Sim)|
| NATUREZA5_DESCRICAO| varchar|	100|	NULL|	Descrição da quinta natureza cadastrada na ocorrência|
| SUBCATEGORIA1_DESCRICAO|	varchar|	70|	NULL|	Descrição da sub-categoria da primeira natureza|
| SUBCATEGORIA2_DESCRICAO|	varchar|	70|	NULL|	Descrição da sub-categoria da segunda natureza|
| SUBCATEGORIA3_DESCRICAO|	varchar|	70|	NULL|	Descrição da sub-categoria da terceira natureza|
| SUBCATEGORIA4_DESCRICAO|	varchar|	70|	NULL|	Descrição da sub-categoria da quarta natureza|
| SUBCATEGORIA5_DESCRICAO|	varchar|	70|	NULL|	Descrição da sub-categoria da quinta natureza|
| OCORRENCIA_ANO|	int|	-|	NOT NULL|	Ano de cadastro da ocorrência|
| OCORRENCIA_CODIGO|	int|	-|	NOT NULL|	Código da ocorrência|
| OCORRENCIA_DATA| datetime|	|-|	NOT NULL|	Data da ocorrência|
| OCORRENCIA_DIA_SEMANA|	varchar|	20|	NOT NULL|	Dia da semana em que a ocorrência foi cadastrada|
| OCORRENCIA_HORA| varchar|	8|	NOT NULL|	Hora em que a ocorrência foi cadastrada|
| OCORRENCIA_MES|	int|	-|	NOT NULL|	Mês em que a ocorrência foi cadastrada|
| OPERACAO_DESCRICAO|	varchar|	70|	NULL|	Nome da operação que realizará o atendimento, caso haja|
| ORIGEM_CHAMADO_DESCRICAO|	varchar|	70|	NOT NULL|	Local em que se originou a chamada|
| REGIONAL_FATO_NOME|	varchar|	20|	NOT NULL|	Regional do fato (local em que ocorreu a ocorrência)|
| SECRETARIA_NOME|	varchar|	70|	NOT NULL|	Nome da secretaria solicitante|
| SECRETARIA_SIGLA|	varchar|	10|	NOT NULL|	Sigla da secretaria solicitante|
| SERVICO_NOME|	varchar|	70|	NOT NULL|	Nome do serviço que realizará o atendimento|
| SITUACAO_EQUIPE_DESCRICAO|	varchar|	70|	NULL|	Situação da equipe no momento atual|
| NUMERO_PROTOCOLO_156|	int|	-|	NULL|	Número do protocolo quando a origem do chamado for 156|


## Organização lógica dos dados 

### 1. Atendimento 

Campos ligados ao momento e ao local básico do atendimento realizado.

- 'ATENDIMENTO_ANO'
- 'ATENDIMENTO_BAIRRO_NOME'

### 2. Localização e contexto 

Campos que ajudam a identificar o logradouro, a existência de equipamento urbano e características associadas ao local.

- 'EQUIPAMENTO_URBANO_NOME'
- 'FLAG_EQUIPAMENTO_URBANO'
- 'FLAG_FLAGRANTE'
- 'LOGRADOURO_NOME'

### 3. Classificação de ocorrência

Campos que descrevem até cinco naturezas da ocorrência e suas respectivas subcategorias. Também informa se cada natureza está associada à defesa civil. 

- 'NATUREZA1_DEFESA_CIVIL' até 'NATUREZA5_DEFESA_CIVIL'
- 'NATUREZA1_DESCRICAO' até 'NATUREZA5_DESCRICAO'
- 'SUBCATEGORIA1_DESCRICAO' até 'SUBCATEGORIA5_DESCRICAO'

### 4. Atendimento e gestão pública 

Campos relacionados à origem do chamado, regional, secretaria, serviço, operação, situação da equipe e protocolo.

- 'OPERACAO_DESCRICAO'
- 'ORIGEM_CHAMADO_DESCRICAO'
- 'REGIONAL_FATO_NOME'
- 'SECRETARIA_NOME'
- 'SECRETARIA_SIGLA'
- 'SERVICO_NOME'
- 'SITUACAO_EQUIPE_DESCRICAO'
- 'NUMERO_PROTOCOLO_156'
