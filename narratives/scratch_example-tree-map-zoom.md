---
title: Demo to explore map + tree zooming
authors: James
date: "Sept 14 2019"
dataset: "https://nextstrain.org/community/jameshadfield/scratch/ncov-demo?d=tree,map"
abstract: "Should start with entire tree & map"
---

# [Display certain branch labels](http://localhost:4000/scratch/ncov-demo?d=tree,map&branchLabel=group)

The nCoV tree annotates some branches with a label of "group".

.

Using a URL query we can show / hide these -- in this case `branchLabel=group`.

.

Notice the "A" and "B" which have appeared?

# [Magically zoom into the tree](http://localhost:4000/scratch/ncov-demo?d=tree,map&label=group:A)

Using those "group" branch labels (which are no longer displayed, since we removed the corresponding query parameter) we can zoom into parts of the tree.

.

Here we've zoomed into group A via `label=group:A`

# [Filters zoom the map](http://localhost:4000/scratch/ncov-demo?d=tree,map&f_country=USA)

Restricting samples to USA means the map automatically zooms.

.

Note also that we zoomed back to the root of the tree by simply removing the `label=group:A` query.

# [China, Taiwan & Thailand sequences](http://localhost:4000/scratch/ncov-demo?d=map&f_country=China,Taiwan,Thailand&r=country)

Data subsetted using filters.

.

Geographic resolution = country.

# [China, Taiwan & Thailand sequences, finer geographic resolution](http://localhost:4000/scratch/ncov-demo?d=map&f_country=China,Taiwan,Thailand&r=loaction)

Switching to viewing "location". Note how the map automatically resizes.

# [Show me amino acid mutations](http://localhost:4000/scratch/ncov-demo?branchLabel=aa&d=tree&m=num_date)

Note how much branching is coming from the coalescent!

.

Queries: `branchLabel=aa` and `m=num_date`
