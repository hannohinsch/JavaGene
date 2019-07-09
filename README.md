# JavaGene
JavaGene is a small set of Java classes for genomic sequence analysis that support fluent programming.

It has excellent support for the low-level sequence manipulations needed when writing gene finders, analyzing gene structure, modeling molecular evolution and similar projects. It's not for annotation pipelines or integrating disparate data sources.

JavaGene completely encapsulates tedious sequence arithmetic, eliminating pesky off-by-one bugs and edge condition error checking, and generally makes working with stranded sequences a breeze.

I originally wrote this for my own use while studying bioinformatics at the University of Pennsylvania, and used it there for three good-sized research projects. The version here is a refactored subset.

#### Overview
• Simple! Documented! Includes sample programs!

• Encapsulates common sequence data types and operations; supports chained, fluent programming.

• Implements a rich set of methods to manipulate locations on a sequence, such as "sliding window" iterators, prefix( ), suffix( ), contains(), distance( ), overlaps(), upstream(), union(), and many more like it.

• Transparently handles operations on forward and reverse strands.

• Supports Fasta format sequence files. Seamlessly supports both typical in-memory sequences and oversized gigabyte-sized sequences (using memory-mapped io).

• Supports various flavors of GFF/GTF feature files. Supports selection of features such as genes, exons, etc based on attributes. Can splice a sequence based on a list of features.

• AminoAcid utilities: Translate nucleotides to amino acids. Check for synonyms. Find Blosum62 distance.

• Nucleotide utilities: Complementation for both DNA and RNA sequences. Check for matches using the IUPAC "ambiguous" symbols, such as R,Y,A, etc.

