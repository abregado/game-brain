---
title: "BS - Procedure Plants"
source: "Game Stuff/Game Ideas/BS - Procedure Plants"
modified: 2013-06-12
type: design-doc
area: other
status: "idea"
projects: []
concepts: ["Procedural Plants Generator"]
words: 341
summary: "Spec for procedurally generated tree species: trunk, root, leaf, bark, bud, flower and fruit parameters, stored lifecycle stages for forest rendering."
tags: ["area/other", "type/design-doc"]
---

Procedurally generated tree species

The idea is to generate random tree species by specifying certain parameters (or randomising all parameters). The system generates an example of the full grown tree in the following parts/order: Trunk+Branches, Roots, Leaves, Flowers/Fruit/Pods. Once the user designates a tree to be completely generated, 3-5 examples of the tree will be created and each stage of its life will be recorded as a single frame of animation. The animation of each specimen growing can then be viewed.

During gameplay a varied forest can be rendered by placing the different specimen of the same species at differnt orientations and stages of its life cycle. Also Flowers/Buds/Leaves will alos be dependant on day/night cycle and seasonal times. This should create a very vibrant and dynamic environment.

With just a few differnt species I beleive this could be very successful at creating interesting forests.

Generate Trunk and Branch Contraints

- Number of branchings at the same node

- Minimum distance before branching

- Maximum angle variance

- Number of trunks at base? (bush/tree)

- Straightness of trunks

- Wind effected?

- Uniform bending

- Trunk:Branch:Root mass ratio

- Grows towards?

- Thorns?

> Generate Leaf Locations

- Minimum height from ground

- Minimum number of leaves at age

- Branching point leaves?

> Generate Root structure

- Root efficency (root:branch ratio)

- Maximum height (if above ground roots)

- Max Thickness/Variance

> Generate Bark

- Pattern

- Thickness

- Roughness

- Coloration

- Moss/Algae

- Ribbing (vertical/horizontal)

- Thorns

> Generate Budding locations

- Trunk/Stem or Branches only

- Minimum branch age for budding

- At branching points?

- At Tips?

- Bud clustering (numbver of clusters, number in cluster)

> Leaf Shape and texture

- Round/Oval/Diamond Shape

- Spine/Ribbing

- Surface details

- Edge details

- Curling?

- Color

- Seasonal Growth/Change

Flower Generation

- LOD!!!!

- Petalaled Flower/Pod/Fruit/Single Petal/Fractal

- Open at night?

- Seasonal Opening?

- Seasonal Coloration Change?

- Budding times?

- Size/Diameter/Mass Variation

- Frond quantity/Length

- Fruit shape (Round/Dual GLobe/Pear/Hourglass/Gourd)

- Length/Diameter of fruit
