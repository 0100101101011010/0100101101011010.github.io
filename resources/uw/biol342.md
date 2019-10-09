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

## Lecture 4:

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

- B and C are likely different from D, E, F
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

## Lecture 9

### W3 Q3

1. purify the protein (grow lots of fungus, centrifuge and purify) and find its sequence
  - amino acid degradation
  - immunoscreening (use antibody, needs lots of protein to work)
  - substrate screening (if your host cells for the library can express the protein, and the protein produces a visible effect)
1. make a *genomic* library
  - can't make a cDNA library because you want both the exons *and* introns (since fungi are eukaryotic), not to mention you also want the promoter, terminator, +1 site, start and stop codons, etc.
1. find the gene of interest from the library (2 ways):
  1. hybridize a probe to the gene (made using the sequence determined from the purified protein)

### W3 Q4

the zebra protein could not be expressed in the host e. coli because:

- the eukaryotic promoter wouldn't be recognized by the bacterial host → no mRNA transcript is even produced
- even if the insert is added to an existing promoter on the vector, there is no shine-dalgarno sequence for initiating translation → no protein is produced
- the eukaryotic promoter sequence and the 5' UTR would be translated into the final protein, resulting in either an out-of-frame translation or a protein with additional amino acids attached

cannot use PCR because you would have to do it for waaaay too many colonies, no time for that!

so, can only use hybridization with probe

### Chemical Synthesis of DNA

in the lab, not natural

#### Phosphoramidite Method

only works for synthesizing small genes (<120 bp)

1. start with linkage of a spacer chain to a solid support (often glass or silicon bead) to prevent the growing chain from being washed away
1. synthesize DNA in the 3' to 5' direction (adds bases to the 5' carbon of the sugar on the 5' end)
  - exact opposite of natural DNA synthesis
1. before adding the next nucleoside, remove DMT, leaving an exposed 5' OH
  - low efficiency... lots of 5' OH groups remain unreacted
1. block off all unreacted 5' OH groups
  - otherwise, you'll end up with incorrectly-sequenced DNA (that have missing bases)
  - capped using acetylation (ends capped with DMT will not be acetylated, thus are protected and can go on to have more bases added)
  - these capped 5' OH groups ensure that the chain they are on does not progress to the next addition
1. synthesize each strand of the DNA helix separately, then anneal them

coupling efficiency: how many of the chains will be full-length (not capped off prematurely)

- (% efficiency of each cycle)^(number of bp in the sequence) = % of chains formed that will be full-length

eg. for a 20-unit DNA sequence (ie. 20-mer) with a 99% coupling efficiency at each cycle:

- 0.99^20 × 100%
- = 82% yield of full-length chains

can only make chains of ~120 bp (50% of the chains formed will be full-length) because of the low efficiency; diminishing returns

#### Modular DNA Synthesis

for larger genes that can't be synthesized in one go by phosphoramidite method

1. synthesize modular fragments of the gene using phosphoramidite method, each at <120 bp, designed so that each one has complementary ends with the next fragment
1. anneal fragments

problem: you can end up with a lot of false matches (fragments joining in the wrong order), so have to sequence the gene after obtaining product

#### PCR

still has the issue of incorrectly-ordered fragments, but reduces this risk because you can *control* the temperature, preventing many of the side annealings

linker = short, blunt-ended double-ended DNA fragment with palindromic strands that contain a recognition site

- when it is ligated into your DNA fragment, then digest, you'll get sticky ends!
