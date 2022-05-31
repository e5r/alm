```
./ERLIMAR.COM
 │ 
 ├─ Managements/
 │  ├─ Area1/
 │  │  └─ Workitem1	ERLIMAR.COM/Managements/Area1
 │  │
 │  ├─ Area2/
 │  ├─ Workitem2	ERLIMAR.COM/Managements
 │  ├─ Workitem3	ERLIMAR.COM/Managements
 │  └─ Workitem4	ERLIMAR.COM/Managements
 │
 ├─ Teams/
 │  ├─ Genesis/
 │  │  └─ Workitem5	ERLIMAR.COM/Teams/Genesis
 │  │
 │  ├─ Ghost/
 │  │  └─ Workitem6	ERLIMAR.COM/Teams/Ghost
 │  │
 │  ├─ Support/
 │  │  └─ Workitem7	ERLIMAR.COM/Teams/Support
 │  │
 │  └─ Workitem8	ERLIMAR.COM/Teams
 │
 └─ Workitem9		ERLIMAR.COM
```

Notas
=====
* [ERLIMAR.COM] Quando um item ainda não foi avaliado de forma alguma
* [ERLIMAR.COM/Teams] Quando um item é desenvolvido sem um time específico
* [ERLIMAR.COM/Teams/X] Quando um item pertence a um time específico
* [ERLIMAR.COM/Managements] Quando um item está na fila de planejamento
* [ERLIMAR.COM/Managements/Area1] Quando um item está planejado por uma área


Epic (Épico)
============
```
Área: Gerenciamento
Responsável: Donos de produto (Ex: Diretoria)
Prazo: Tem prazo definido

Metas de alto nível. Um objetivo a ser alcançado.
Ex: Suporte a nova legislação 2022
```

Feature (Recurso)
=================
```
Área: Gerenciamento
Responsável: Equipe de recurso (Ex: Analistas de negócio)
Prazo: Tem prazo definido

Um recurso agrupa funcionalidades semelhantes e descrevem o objetivo
mais claramente.
```

Product Backlog Item (Item)
==========================
```
Área: Time de recursos
Responsável: Equipe de recurso (Ex: Analistas de sistema)
Prazo: Não tem prazo definido

Parte entregável de um recurso que pode ser especificada
```

Task (Tarefa)
=============
```
Área: Time de recursos
Responsável: Desenvolvedor
Prazo: Não tem prazo definido

Uma atividade bem definida que pode ser feita de forma independente.
```

Impediment (Impedimento ou Problema)
====================================
```
Área: Time de recursos
Responsável: Desenvolvedor
Prazo: Não tem prazo definido

Um problema ou impedimento que precisa ser resolvido para o bom
andamento das demais atividades, mas que não está diretamente
relacionada a uma história de usuário ou recurso específico.
Ex: Configuração de ambiente. Provisionamento de base de dados.
```
