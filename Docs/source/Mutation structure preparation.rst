Mutation structure preparation
--------------------------------


[G2S](https://g2s.genomenexus.org) provides a real-time web API that provides an automated mapping of genomic variants on 3D protein structures. G2S can align genomic locations of variants and protein sequences to protein structures and retrieve the mapped residues from matched structures of genomic variants. We systematically queried G2S to obtain mutation-based structures aligning to the input sequence. Giving protein sequence and the position of a variant as the query (Figure 2B), G2S searches matched genomic variants and gets a list of protein structures of genomic variants as mutation-based residue-level structures. We divided this list of protein structures of genomic variants based on the type of the wild-type and mutant amino acids based on the query sequence (Figure 2A).  Due to the availabilities of the PDB structures, four categories of PDB structures are adopted (Figure 2A). Q1: Tertiary structures of matched proteins with wild-type residue and with mutant residue are both available. Q2: Tertiary structures of matched proteins with wild-type residue are available and tertiary structures of matched proteins with mutant residue are unavailable. Q3: Tertiary structures of matched proteins with wild-type residue are unavailable and tertiary structures of matched proteins with mutant residue are available. Q4: Tertiary structures of matched proteins with wild-type residue and with mutant residue are both unavailable. Here, we used mutation-based background knowledge to replace both wild-type and mutation structure information in Q4, an average of values of tertiary structure which are the total variant structures form residue one to another according to wild-type and mutation residue on the query in G2S. For example, the tertiary structure of protein CspB-TB in the S1676 dataset is unavailable. When searching it in G2S, it cannot align a suitable structure, neither wild-type nor after mutation. Therefore, we use mutation-based background knowledge to get mutation-based residue-level structure features to make up for missing structures.


![](https://raw.githubusercontent.com/hurraygong/SCpre-seq/master/pictures/Figure_1.png)




