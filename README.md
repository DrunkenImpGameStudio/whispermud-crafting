# complex-crafting

A more complex crafting bundle for RanvierMUD.

## Current features

- Resource-based crafting (similar to simple-crafting)
- Item-based crafting (consumes existing inventory items to create a new one)
- Tools (items that you need for a recipe but are not consumed)
- Enhanced crafting commands such as craft search
- Initial support for concepts such as 'blueprints' or learning recipes.

## Crafting

Recipes are defined in 'data/recipes.md' like so:

```
- item: "limbo:7" # target item to create
  recipe:
    plant_material: 3 # resource key: amount
    rose_petal: 1
```

For the player to get resources you'll need two things: one is to define the resource type in 'data/resources.yml'.
Second is to create a node for them to gather from. See areas/craft/items.yml for examples.