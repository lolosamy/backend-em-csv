# Evidências - INSERT, UPDATE e DELETE no banco db_em
## Identificação
Nome: Lorena Samyra
Turma: 3b
Data: 19/05/2026
---
# 1. SELECT final - Leituras do dia 2026-04-04
Execute no DBeaver:

Trilha CRUD SQL - db_em - DBeaver

```sql
SELECT *
FROM leituras
WHERE timestamp >= '2026-04-04'
AND timestamp < '2026-04-05'
ORDER BY timestamp ASC;
```
Cole abaixo a saída obtida:
```text
cole aqui a saída do SELECT
```
1	EM-ARACATUBA-01	2026-04-01 08:00:00.000 -0300	24.5
2	EM-ARACATUBA-01	2026-04-01 09:00:00.000 -0300	25.8
3	EM-ARACATUBA-01	2026-04-01 10:00:00.000 -0300	27.2
4	EM-ARACATUBA-01	2026-04-02 08:00:00.000 -0300	23.9
5	EM-ARACATUBA-01	2026-04-02 09:00:00.000 -0300	25.1
6	EM-ARACATUBA-01	2026-04-02 10:00:00.000 -0300	26.7
7	EM-ARACATUBA-01	2026-04-02 08:00:00.000 -0300	23.8
8	EM-ARACATUBA-01	2026-04-02 09:00:00.000 -0300	24.6
9	EM-ARACATUBA-01	2026-04-02 10:00:00.000 -0300	25.4
10	EM-ARACATUBA-01	2026-04-02 11:00:00.000 -0300	26.1
11	EM-ARACATUBA-01	2026-04-02 12:00:00.000 -0300	27.0
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9
---
# 2. SELECT final - Conferência do UPDATE
Execute no DBeaver:
```sql
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 09:00:00';
```
Cole abaixo a saída obtida:
```text
cole aqui a saída do SELECT
```
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5

---
# 3. SELECT final - Conferência do DELETE
Execute no DBeaver:
```sql# Evidências - INSERT, UPDATE e DELETE no banco db_em
## Identificação
Nome:
Turma:
Data:
---
# 1. SELECT final - Leituras do dia 2026-04-04
Execute no DBeaver:

Trilha CRUD SQL - db_em - DBeaver

```sql
SELECT *
FROM leituras
WHERE timestamp >= '2026-04-04'
AND timestamp < '2026-04-05'
ORDER BY timestamp ASC;
```
Cole abaixo a saída obtida:
```text
cole aqui a saída do SELECT

12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5
```
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5

---
# 2. SELECT final - Conferência do UPDATE
Execute no DBeaver:
```sql
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 09:00:00';
```
Cole abaixo a saída obtida:
```text
cole aqui a saída do SELECT
```
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5
---
# 3. SELECT final - Conferência do DELETE
Execute no DBeaver:
```sql
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 11:00:00';
```
Cole abaixo a saída obtida:
```text
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5

Trilha CRUD SQL - db_em - DBeaver

cole aqui a saída do SELECT

```
Se o DELETE foi feito corretamente, esse SELECT não deverá retornar registros.
---
# 4. SELECT final - Todas as leituras ordenadas
Execute no DBeaver:
```sql
SELECT *
FROM leituras
ORDER BY id ASC;
```
Cole abaixo a saída obtida:
```text
cole aqui a saída do SELECT
```
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5
---
# 5. Teste pela API
Acesse no navegador:
```text
http://localhost:3000/api/leituras/data/2026-04-04
```
Cole abaixo o resultado retornado pela API:
```json
{
  "dataPesquisada": "2026-04-04",
  "total": 4,
  "leituras": [
    {
      "id": 12,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T11:00:00.000Z",
      "temperature_c": 23.4,
      "humidity_pct": 76.2
    },
    {
      "id": 13,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T11:00:00.000Z",
      "temperature_c": 23.4,
      "humidity_pct": 76.2
    },
    {
      "id": 14,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T12:00:00.000Z",
      "temperature_c": 25.2,
      "humidity_pct": 72
    },
    {
      "id": 15,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T13:00:00.000Z",
      "temperature_c": 25.9,
      "humidity_pct": 70.5
    }
  ]
}


cole aqui o resultado da API
```

{
  "dataPesquisada": "2026-04-04",
  "total": 4,
  "leituras": [
    {
      "id": 12,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T11:00:00.000Z",
      "temperature_c": 23.4,
      "humidity_pct": 76.2
    },
    {
      "id": 13,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T11:00:00.000Z",
      "temperature_c": 23.4,
      "humidity_pct": 76.2
    },
    {
      "id": 14,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T12:00:00.000Z",
      "temperature_c": 25.2,
      "humidity_pct": 72
    },
    {
      "id": 15,
      "station_id": "EM-ARACATUBA-01",
      "timestamp": "2026-04-04T13:00:00.000Z",
      "temperature_c": 25.9,
      "humidity_pct": 70.5
    }
  ]
}

---
# 6. Conclusão
Explique com suas palavras a diferença entre INSERT, UPDATE e DELETE.
Resposta:
INSERT: Serve para inserir novas linhas (ou registros) em uma tabela. Você especifica em quais colunas deseja colocar os dados e quais serão os valores.
UPDATE: Serve para modificar dados que já existem em uma tabela. Você usa filtros (geralmente com  WHERE) para indicar exatamente qual linha deve ser alterada e define os novos valores.
DELETE:remove linhas existentes de uma tabela. Assim como no UPDATE, você deve usar um filtro (como WHERE) para apagar apenas os registros desejados, caso contrário, apagará todos os dados da tabe
Trilha CRUD SQL - db_em - DBeaver

```
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 11:00:00';
```
Cole abaixo a saída obtida:
NADA

Trilha CRUD SQL - db_em - DBeaver

cole aqui a saída do SELECT
```
Se o DELETE foi feito corretamente, esse SELECT não deverá retornar registros.
---
# 4. SELECT final - Todas as leituras ordenadas
Execute no DBeaver:
```sql
SELECT *
FROM leituras
ORDER BY id ASC;
```
Cole abaixo a saída obtida:
1	EM-ARACATUBA-01	2026-04-01 08:00:00.000 -0300	24.5	72.1
2	EM-ARACATUBA-01	2026-04-01 09:00:00.000 -0300	25.8	69.4
3	EM-ARACATUBA-01	2026-04-01 10:00:00.000 -0300	27.2	65.8
4	EM-ARACATUBA-01	2026-04-02 08:00:00.000 -0300	23.9	74.3
5	EM-ARACATUBA-01	2026-04-02 09:00:00.000 -0300	25.1	70.6
6	EM-ARACATUBA-01	2026-04-02 10:00:00.000 -0300	26.7	67.2
7	EM-ARACATUBA-01	2026-04-02 08:00:00.000 -0300	23.8	73.5
8	EM-ARACATUBA-01	2026-04-02 09:00:00.000 -0300	24.6	71.2
9	EM-ARACATUBA-01	2026-04-02 10:00:00.000 -0300	25.4	68.9
10	EM-ARACATUBA-01	2026-04-02 11:00:00.000 -0300	26.1	66.4
11	EM-ARACATUBA-01	2026-04-02 12:00:00.000 -0300	27.0	63.8
12	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
13	EM-ARACATUBA-01	2026-04-04 08:00:00.000 -0300	23.4	76.2
14	EM-ARACATUBA-01	2026-04-04 09:00:00.000 -0300	25.2	72.0
15	EM-ARACATUBA-01	2026-04-04 10:00:00.000 -0300	25.9	70.5
cole aqui a saída do SELECT
```

---
