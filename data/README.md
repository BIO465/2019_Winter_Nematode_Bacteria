Dana—

Here are two Excel files with your output. “i” stands for input and “b” stands for blendate from insects. The “n” designation for your sample names denotes that the data have been normalized, so the total hops per condition in the whole genome will be equal. There has been no normalizing wrt gene length, since you are comparing across conditions, not genes.

The first file (10_13genes) shows the number of hops on a per-gene basis. You can see that I have added a fitness column to reflect how well mutants for each gene fared in the host: [(avg of b3 and b4)/(avg of i1 and i2)]. So a low score reflects poor competition in the insect.

The second file (10_13hopsites) breaks down the hops into the individual sites where those hops occurred. Because your library was limited in size, you will see that many genes only had a single hop site, though the hop counts for that site may be high (in the hundreds); many genes have no hop sites, but this does not necessarily mean they are essential for viability—I’m sure many genes are transposon-free simply because the library was small.

All-in-all, you should be excited about the data. There is pretty good agreement between replicates, and I’m sure that of the hundreds of genes that register a strongly decreased fitness in the insect, many of these genes may truly contribute to host colonization. The best way to narrow down the best candidates from here would be to identify genes in this category where multiple insertion sites are telling the same story. For example: Gene 209 from the “genes” file looks promising…until you go to the “hopsites” file and see that 209 only has one hop site. On the other hand, gene 1886 looks more promising because the low fitness is supported by two major hop sites. Of course, another criterion would be reproducibility across replicates. For example, if you look at Gene 4506, you can see some reproducibility issues. You may want to come up with a set of criteria for composing a final list of candidates, such as:

1. Fitness less than or equal to 0.2
2. Deviation between replicates not greater than (some number)
3. Fitness score supported independently by at least two hop sites in the gene

Anyway, enjoy analyzing, and let me or Ryan know if you want any more tips.

Joel
