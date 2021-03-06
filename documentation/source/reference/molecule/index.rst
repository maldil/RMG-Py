*************************************************
Molecular representations (:mod:`rmgpy.molecule`)
*************************************************

.. module:: rmgpy.molecule

The :mod:`rmgpy.molecule` subpackage contains classes and functions for working
with molecular representations, particularly using chemical graph theory.



Graphs
======

.. currentmodule:: rmgpy.molecule.graph

======================= ========================================================
Class                   Description
======================= ========================================================
:class:`Vertex`         A generic vertex (node) in a graph
:class:`Edge`           A generic edge (arc) in a graph
:class:`Graph`          A generic graph data type
======================= ========================================================



Graph isomorphism
=================

.. currentmodule:: rmgpy.molecule.vf2

======================= ========================================================
Class                   Description
======================= ========================================================
:class:`VF2`            Graph isomorphism using the VF2 algorithm
======================= ========================================================



Elements and atom types
=======================

.. currentmodule:: rmgpy.molecule

======================= ========================================================
Class/Function          Description
======================= ========================================================
:class:`Element`        A model of a chemical element
:func:`get_element`     Return the :class:`Element` object for a given atomic number or symbol
:class:`AtomType`       A model of an atom type: an element and local bond structure
:func:`get_atomtype`    Return the :class:`AtomType` object for a given atom in a molecule
======================= ========================================================



Molecules
=========

.. currentmodule:: rmgpy.molecule

======================= ========================================================
Class                   Description
======================= ========================================================
:class:`Atom`           An atom in a molecule
:class:`Bond`           A bond in a molecule
:class:`Molecule`       A molecular structure represented using a chemical graph
======================= ========================================================



Functional groups
=================

.. currentmodule:: rmgpy.molecule

======================= ========================================================
Class                   Description
======================= ========================================================
:class:`GroupAtom`      An atom in a functional group
:class:`GroupBond`      A bond in a functional group
:class:`Group`          A functional group structure represented using a chemical graph
======================= ========================================================



Molecule Utilities
==================

.. currentmodule:: rmgpy.molecule

================================ ========================================================
Class                            Description
================================ ========================================================
:mod:`rmgpy.molecule.resonance`  Resonance structure generation methods
:mod:`rmgpy.molecule.kekulize`   Kekule structure generation
:mod:`rmgpy.molecule.filtration` Resonance structure filtration methods
:mod:`rmgpy.molecule.pathfinder` Resonance path enumeration
:mod:`rmgpy.molecule.converter`  Molecule object converter (RDKit/OpenBabel)
:mod:`rmgpy.molecule.translator` Molecule string representation translator
================================ ========================================================



Adjacency lists
===============

.. currentmodule:: rmgpy.molecule.adjlist

=========================== ====================================================
Function                    Description
=========================== ====================================================
:func:`from_adjacency_list` Convert an adjacency list to a set of atoms and bonds
:func:`to_adjacency_list`   Convert a set of atoms and bonds to an adjacency list
=========================== ====================================================



Symmetry numbers
================

.. currentmodule:: rmgpy.molecule.symmetry

======================================== ========================================
Class                                    Description
======================================== ========================================
:func:`calculate_atom_symmetry_number`   Calculate the atom-centered symmetry number for an atom in a molecule
:func:`calculate_bond_symmetry_number`   Calculate the bond-centered symmetry number for a bond in a molecule
:func:`calculate_axis_symmetry_number`   Calculate the axis-centered symmetry number for a double bond axis in a molecule
:func:`calculate_cyclic_symmetry_number` Calculate the ring-centered symmetry number for a ring in a molecule
:func:`calculate_symmetry_number`        Calculate the total internal + external symmetry number for a molecule
======================================== ========================================



Molecule and reaction drawing
=============================

.. currentmodule:: rmgpy.molecule.draw

======================== =======================================================
Class                    Description
======================== =======================================================
:class:`MoleculeDrawer`  Draw the skeletal formula of a molecule
:class:`ReactionDrawer`  Draw a chemical reaction
======================== =======================================================



.. toctree::
    :hidden:
    
    vertex
    edge
    graph
    vf2
    element
    atomtype
    recipe
    atom
    bond
    molecule
    groupatom
    groupbond
    group
    resonance
    kekulize
    filtration
    pathfinder
    converter
    translator
    adjlist
    symmetry
    moleculedrawer
    reactiondrawer
