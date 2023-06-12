# Wazuh - Comandos de API


## Acesse o módulo de desenvolvimento

```
https://IP_WAZUH_DASHBOARD/app/wazuh#/wazuh-dev?tab=devTools
```

Utilize os comandos abaixo para efetuar as ações nos agentes:

## Atualizar todos os agentes
```
PUT /agents/upgrade?agents_list=all
```
## Atualizar agente individual
```
PUT /agents/upgrade?agents_list={Agent ID}
```
## Requisitar dados do Agente
```
GET /agents?agents_list={Agent ID}
```
## Inserir um agente no Grupo
```
PUT /agents/{Agent ID}/group/{Grupo}
```
## Remover um agente no Grupo
```
DELETE /agents/{Agent ID}/group/{Grupo}
```
## Restart agente
```
PUT /agents/restart?agents_list={Agent ID}
```
## Remover host
```
DELETE /agents?agents_list={Agent ID}
```
## Remover host (forçado)
```
DELETE /agents?agents_list={Agent ID}&status=disconnected&older_than=0d
```
