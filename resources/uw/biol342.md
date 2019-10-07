# BIOL 342

## Lecture 1: Review

monocistronic = only 1 gene in the mRNA

polycistronic: each gene has its own ribosome-binding site (SD + AUG)

polycistronic mRNA is not an operon because there is no control (no operator present on the gene) they are constitutive, aka housekeeping, genes

- genes become blurry... in an operon, only one promoter and one terminator controls production of *several proteins*... however, they are typically still considered distinct genes rather than one gene coding for several proteins

- shine-dalgarno isn't right at the 5' end, there's some space
- then some more space between SD and start codon (usually ~6–10 bp)
- in most cases, the fM (translated from the start codon) is cleaved off in post-translational processing

### POST-TRANSCRIPTIONAL MODIFICATION

- 5' guanine cap
- 3' polyadenine tail: contributes to stability

### POST-TRANSLATIONAL MODIFICATION

- often, Met/fMet is removed

## Lecture 2: Review

### STRUCTURAL DIFFERENCE BETWEEN DNA AND mRNA

- mRNA does not have Promoter or Terminator (those belong to DNA only)—well, part of the Terminator remains, but not the entire thing
- start codon in mRNA is AUG, not ATG (also ATG has no impact on DNA)
- shine-dalgarno sequence exists in both, but only has an impact on translation (mRNA → protein)
- codons are only ever in the CDS / ORF
  - eg. cannot call the nucleotides in the SD a codon, because that region is not translated
  - start codon is included in ORF; stop codon is not included in ORF

### ORIGIN OF REPLICATION

- eukaryotes have much bigger genomes, so require multiple origins of replication to replicate DNA in a timely manner
- bacteria can do with just one origin

## Lecture 3:

**important!!** bacteria used as host cells for vectors must be *defective* in the restriction endonuclease for the cut site you selected. otherwise, once you clone an insert-containing vector into the cell, it would just recognize that site and cut it up, destroying the vector you worked so hard on.

### CUTTING DNA

- restriction endonucleases have the advantage because they cut at precise, predetermined sites, and they produce hanging ends
- mechanical methods of cutting DNA are more random: hard to reproduce, hard to control, produces blunt ends
  - sonicate (shear it)
  - glass beads (bead beater)
  - small needle

### RFLP Analysis

- for finding genetic differences between *closely related strains*
- useful in epidemiology: tracing movement of pathogen strains through a population
  - eg. you can see if a particular disease arose from one origin, or multiple foci

#### how it works

- tests *DNA*
- digest entire genome with a specific suite of restriction enzymes
- look for differences in the resulting pattern → different bands mean that there's a differing number of bps between the same restriction sites → the sequence between those two organisms in that region is different

#### what does the presence of a different-looking band mean?

possibilities:

- there was a deletion or SNP in the restriction site, therefore removing it (the enzymes no longer recognize)
- transposons: less bands, that are smaller
- insertion that causes a new restriction site: more, smaller bands

![rflp analysis](/resources/uw/images/rflp.jpg){:width="100%"}

in image above:

- B and C are likely different from D, E F
- D and F are likely different from E
- E is more similar to F than D

** careful not to use the phrase "the same" in describing the bands, because they are likely not the same (RFLP cannot tell us that level of detail)

### Cloning Vectors

#### size

naturally occuring plasmids range from 1 kb to >500 kb! (however, the ones used for cloning are usually small (<12 kb))

larger plasmids can hold more genetic information, but are also more metabolically demanding

#### copy number

multiple copies of a plasmid will exist in the host, usually from <10 to >100 copies

some low-copy number plasmids contain information to ensure they will be distributed to all new daughter cells (segregation). this ensures they are perpetuated, otherwise, they would quickly be lost within a population.

#### expression vs cloning vectors

### Cloning Vectors

#### features of all modern cloning vectors

- origin of replication (eg. OriC in e. coli)
- selectable marker (ampicillin resistance gene, tetracycline, etc.) OR screening marker (galactosidase gene, etc.)
- multiple cloning site (MCS)
- small size
- high copy number (this goes hand in hand with small size. if the size is big the cell will have a hard time getting the energy to maintain so many copies)

#### example: pBR322

what is the best site to use on this plasmid if you are going to clone a DNA fragment into it?

![pBR322 plasmid](/resources/uw/images/pbr322.jpg){:width="100%"}

can choose PstI if you want to knock out the Amp resistance gene, or HindIII / BamHI / SalI if you want to knock out the Tet resistance gene. don't knock out both genes (eg. PstI *and* HindIII) or you will not be able to select

what are the steps for cloning?

1. choose restriction site (let's go with PstI)
1. ligate insert into vector
1. transform vector into cells using electroporation (most efficient) or CaCl2
1. *screen for vector*. plate on tetracycline (since the PstI site is not located on the Tet resistance gene, the Tet resistance gene was not cleaved and thus successfully transformed cells will be Tet resistant, and will grow on the plate)
1. *screen for insert*. create a replica plate containing ampicillin. now the cells containing insert (who have had their Amp resistance gene cleaved) will die on the ampicillin plate. compare the Amp and Tet plates. the colonies missing from the Amp plate are the ones containing the insert, and you can pick them off from the Tet plate for amplifying.

### Double Digest vs Single Digest

advantages of double digest:

- prevent self ligation, increases transformation efficiency
- orientation and directional cloning

how to distinguish cells carrying self-ligated vectors from cells carrying desired DNA fragment:

- design polymerase to vector sequence
- run colony PCR

pUC19 advantages:

- multiple cloning site (MCS)
  - lots of choice of sites
  - helps prevent self-ligations
  - facilitates directional cloning (can only go one way)
- can do colour differentiation as well as antibiotic selection
  - LacZ gene will either be disrupted
- very small size, and very high copy number

### W3 Q3

- purify the protein (grow lots of fungus, centrifuge and purify) and find its sequence
  - amino acid degradation
- can't make a cDNA library because you want the introns, so make a *genomic* library
- hybridize a probe to the gene (made using the sequence determined from the purified protein)

### W3 Q4

- cannot use PCR because you would have to do it for waaaay too many colonies, no time for that!
-
