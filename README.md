# Research Project 2 proposal: A Living Forest

**Unreal Engine 5.8 (C++, StateTree AI, NavMesh) + Houdini 22 for the animal models**

## The project in one sentence

I'll turn my Interactive World Builder forest into a real sandbox game: low-poly animals that live on their own (they eat, sleep, flee, hide from storms) and that you can befriend by feeding them, plus gathering, crafting and building, so you can collect wood, stone and berries, make tools and food, and build your own camp in the generated forest.

## Why this one

Go deep. My forest is beautiful and its sky is alive, but nothing lives in it and there is nothing to do yet. Afterward I'll be able to:

- build game AI in Unreal: StateTree (or Behavior Trees), NavMesh, perception, needs that drive behavior;
- write real gameplay systems in C++: inventory, crafting recipes, placing buildings in the world, saving and loading;
- animate low-poly creatures, first with procedural motion in code, then with simple rigs.

## What I'll show

The game. In a freshly generated forest, deer graze, rabbits hide when the storm comes, the fox sleeps at night. I gather berries and wood, craft a basket and a campfire, feed a rabbit until it trusts me and follows me home to my camp. Plus a short breakdown of the AI logic and the crafting system.

## The three weeks

- **By Dec 1:** one animal (rabbit) wanders on the NavMesh and flees the player. Inventory works: pick up wood, stone, berries, apples. Feeding works.
- **By Dec 8:** needs (hunger, sleep, fear) drive the animals; they react to rain, storms and night from my living sky. Trust grows when you feed an animal, and a tame one follows you. Crafting: a few recipes (campfire, basket, fence, simple cabin pieces) and placing them in the world with a preview.
- **By Dec 14:** 3 species with different personalities (rabbit, deer, fox), procedural animation (hop, walk, head turn), save/load of the camp and tamed animals, sounds, polish, video.

## The smallest version that still counts

One species that wanders, flees, sleeps at night, hides in the rain and can be tamed by feeding it, plus picking things up and crafting/placing one object (a campfire).

## The riskiest part

**Animation.** Rigging and skeletal animation for low-poly animals is new to me, so I'll start with procedural motion in code and add skeletal animation only if time allows. Second risk: **scope.** Animals and building are two systems, so the animals come first and building grows on top. Third: the NavMesh has to rebuild correctly every time the World Builder regenerates the terrain.

Game repo: [Midterm-a-tool-you-d-actually-use](https://github.com/elisedumaine/Midterm-a-tool-you-d-actually-use)
