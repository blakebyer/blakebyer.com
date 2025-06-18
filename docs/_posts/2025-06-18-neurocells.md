---
title: Cells of the Nervous System
date: 2025-06-18
layout: single
categories: [blog]
excerpt: "An overview of cells in the nervous system."
---
## Levels of Organization of Multicellular Organisms ##
In order from smallest to largest, the body is composed of:
1. Organelles: cellular components built for specific functions (e.g. endoplasmic reticulum).
2. Cells: basic subunit of biology (e.g. nerve cell).
3. Tissue: a group of similar cells that perform a specific function (e.g. smooth muscle).
4. Organ: many tissue types forming a contiguous body to perform a more complex function (e.g. heart, lungs, or brain).
5. Organ System: a collection of organs that work together to perform a major bodily function (e.g. digestive system).

<figure>
    <img
    src="/assets/images/Organization_levels_mouse.jpg"
    alt="Levels of organization mouse">
    <figcaption><em>
    Organization levels from cell until organism by LadyofHats at English Wikipedia, Public Domain.
    </em><figcaption>
</figure>

## Cells ##
A cell is a basic subunit of tissue within organisms. 

<figure>
    <img
    src="/assets/images/Animal_cell_structure_en.jpg" 
    alt="Typical animal cell">
    <figcaption><em>
    Structure of a typical animal cell by LadyofHats at English Wikipedia, Public Domain.
    </em></figcaption>
</figure>

A typical animal cell is surrounded by a cell (plasma) membrane and has many different organelles. Cells are adapted for their unique function. For instance, red blood cells (RBCs) lack a nucleus and all other organelles such that they can be filled with hemoglobin, a protein that carries molecular oxygen (O<sub>2</sub>) to the tissues.

## Cellular Taxonomy of the Nervous System ##

A basic taxonomy of cells within the nervous system may look like the following:

digraph flowchart {
   graph [layout = dot, rankdir = TB, splines = ortho, fontname = 'Helvetica']

  node [shape = box, style = filled, color = '#D2E3F3', fontcolor = black,
        fontname = 'Helvetica']
  A [label = 'Cell of Nervous System']
  B [label = 'Neuron']
  C [label = 'Glia']
  D [label = 'Cholinergic neuron']
  E [label = 'Dopaminergic neuron']
  F [label = 'Astrocyte']
  G [label = 'Microglia']
  
  A -> B
  A -> C
  B -> D
  B -> E
  C -> F
  C -> G
}
