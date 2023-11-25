This is an example of how to use BLAST. 
The Basic Local Alignment Search Tool is used to compare a target sequence to reference sequences in databases like GenBank. 
It can be used to identify genes, species, and proteins! 
Access it here: [https://blast.ncbi.nlm.nih.gov/Blast.cgi](https://blast.ncbi.nlm.nih.gov/Blast.cgi) 


For this example, I have obtained this amino acid sequence from GenBank. At the end, you will be at the same page I started at. Of course, when you apply this to your own data, it won't necessarily be an exact match like this. 
Here is the FASTA sequence. I have removed the first line, which had the accession number, protein name, and species name. 

MEDAKNIMHGPAPFYPLEDGTAGEQLHKAMKRYAQVPGTIAFTDAHAEVNITYSEYFEMACRLAETMKRY
GLGLQHHIAVCSENSLQFFMPVCGALFIGVGVAPTNDIYNERELYNSLSIGVAPTNDIYNERELYNSLSI
KKLPIIQKIVILDSREDYMGKQSMYSFIESHLPAGFNEYDSTGLPKGVELTHQNVCVRFSHCRDPVFGNQ
IIPDTAILTVIPFHHGFGMFTTLGYLTCGFRIVLMYRFEEELFLRSLQDYKIQSALLVPTLFSFFAKSTL
VDKYDLSNLHEIASGGAPLAKEVGEAVAKRFKLPGIRQGYGLTETTSAIIITPEGDDKPGACGKVVPFFS
AKIVDLDTGKTLGVNQRGELCVKGPMIMKGYVNNPEATSALIDKDGWLHSGDIAYYDKDGHFFIVDRLKS
LIKYKGYQVPPAELESILLQHPFIFDAGVAGIPDPDAGELPAAVVVLEEGKTMTEQEVMDYVAGQVTASK
RLRGGVKFVDEVPKGLTGKIDGRKIREILMMGKKSKL

Follow the link above to get to the BLAST webpage. You could also download it and run it on your computer. 
Click on the "Protein BLAST" option. 
Copy and paste the amino acid sequence I provided above into the first box. 
If we wanted to adjust the parameters of the algorithm that BLAST uses, we could change things like the substitution matrix used to score mismatches, the length of the word chunks that BLAST will break our query sequence into, or many other options. For those first two, we'll just use the default BLOSUM62 matrix and keep the word length at 5. 
Hit the blue BLAST button! 
It should take about a minute, since our query sequence isn't very long. 
The program returns a list of the top matches for our sequence. 
The best one appears to be the luciferase protein of Lampyris noctiluca. You can see that it has a percent identity of 100.00%, though that won't always be the case. It has an E value of 0.0. Generally, you want the E value to be less than 0.05 to reduce the risk of a false positive. 
Click on the top match to see the alignment between our sequence and the reference sequence. They are perfectly aligned in this example. 
Above the alignment, it should say "Sequence ID", followed by a hyperlink saying AAR20794.1. Click it! 
You are now where I started! This is the GenBank entry for the enzyme that makes this firefly glow! 

The process for a nucleotide search is very similar. You'll notice that on this protein's entry, it has a section called "CDS". That is a coding sequence for a protein. In this case that covers the whole entry since this is the entry for the protein itself, but a nucleotide entry may contain zero or multiple coding sequences. You could find a CDS, copy that section, translate it into an amino acid sequence, and search that to just find the protein, though it may also be linked in the CDS. 

I hope this tutorial was helpful. Have a BLAST! 
