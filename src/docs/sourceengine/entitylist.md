# entitylist table

## Functions

## **get_highest_entity_index()**: number

Getting highest entity index
```lua
local idx = entitylist.get_highest_entity_index()
```
---

## **get_local_player()**: number

Getting local player index
```lua
local idx = entitylist.get_local_player()
```
---

## **get_entity_by_index(index)**: [entity_t](../types/entity_t)
Type | Name | Description
------------ | ------------- | ------------
number | index | Entity index

Getting local player by index
```lua
local lp = entitylist.get_entity_by_index(entitylist.get_local_player())
```
---

## **get_entity_by_handle(handle)**: [entity_t](../types/entity_t)
Type | Name | Description
------------ | ------------- | ------------
number | handle | Entity handle

---

## **get_players(type)**: [entity_t](../types/entity_t) array
Type | Name | Description
------------ | ------------- | ------------
number | type | Type

0 - enemies only

1 - teammates only

2 - all players

Getting the enemies array
```lua
  local players = entitylist.get_players(0)
  for i = 1, #players do
      local player = players[i]
  end
```
---

## **get_entities_by_class(classname)**: [entity_t](../types/entity_t) array
Type | Name | Description
------------ | ------------- | ------------
string | classname | Class name

Getting the entities
```lua
  local entities = entitylist.get_entities_by_class("CFogController")
```
---

## **get_entities_by_class_id(classid)**: [entity_t](../types/entity_t) array
Type | Name | Description
------------ | ------------- | ------------
number | classid | Class id

Getting the entities
```lua
  local entities = entitylist.get_entities_by_class(78)
```