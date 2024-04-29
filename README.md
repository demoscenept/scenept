# Página web ScenePT

# Tema original
Baseada no tema [Norlin](https://norlin.netlify.app/).

## Status Deplyment
[![Netlify Status](https://api.netlify.com/api/v1/badges/1390632a-7b4c-4cb6-826d-9835f6f535a7/deploy-status)](https://app.netlify.com/sites/scenept01/deploys)


Notas : O branch **publish** é o que está configurado para deploy via netlify.


## Como usar

### Lista Autores
Os autores estão definidos no ficheiro `_data/authors.json` .
A sua estrutura é definia por um array de objetos , tendo cada objeto 3 campos : 

```json
{
        "id" : "texto",
        "name" : "nome",
        "avatar" : "/images/avatar/xxx.jpg"
}
```


 O campo `id` deve ser igual ao campo `author` no topo de cada post. Isto garante que o nome fica associado a respetiva foto de perfil.

### Como fazer posts

Criar um ficheiro `.markdown` na pasta `_posts`. O cabeçalho têm o seguinte formato (exemplo): 
```---
layout: post
title: "STR Industra Post Mortem"
date: 2021-11-30 19:15:30
categories: post-mortem
tags:   [post-mortem, Vollumetric-Illusions]
image:  '/images/wings_002.jpg'
author: "Jae686"

---
```

As categorias e as tags não estão normalizadas (são definidas por post), pelo , para as categorias, se deve seguir as definições na tabela abaixo para garantir que as mesmas categorias usam o mesmo texto descritivo. 
O nome da categoria não pode conter espaços.

Categorias :

| Nome categoria | Descrição |
|-----|-----------|
|post-mortem| Post-Mortem de demos, projetos ou eventos|
|party-report| Part Reports|
|how-to| how-tos|
---

### Eventos

Os eventos são listados em `_data/events.json` , e a informação guardada é a seguinte : 

```
[
    {
     "title" : "Synergy",
     "date_start" : "2024-05-04",
     "date_end" : "2024-05-05",
     "description" : "Evento realizado com o museu ZX LOAD",
     "local" : "Catanhede"
    },
    {
        "title" : "Inercia Demoparty 2024",
        "date_start" : "TBD",
        "date_end" : "TBD",
        "description" : "Inercia Demoparty",
        "local" : "Almada"
    }
]
```
Para adicionar um Novo evento a tabela, basta acrescentar um novo evento no fim da lista

```
{
        "title" : "Synergy",
        "date_start" : "2024-05-04",
        "date_end" : "2024-05-05",
        "description" : "Evento realizado com o museu ZX LOAD",
        "local" : "Catanhede"
}
```
