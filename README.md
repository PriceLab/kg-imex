# kg-imex
extract IMEx interactions into nodes and edges (entities and
relations), import variously

# TO DO

The *tsv* directory currently (5 jan 2021) holds two version of one
table, intact-human-clean, from which a few lines are shown below,
transposed for easy reading.  A better approach is to transform
IMEx/IntAct into *two* files, one for the entities (proteins), one for
the relationships (interactions). 


<pre>
A                                              Q8IYT4                               Q9BW62                               Q5S007
B                                          A0A024QZP7                           A0A024QZP7                           A0A024QZS4
method                     tandemAffinityPurification           tandemAffinityPurification         antiTagCoimmunoprecipitation
type                                      association                          association                          association
idMethod.A                  sequenceTagIdentification            sequenceTagIdentification            sequenceTagIdentification
idMethod.B                  sequenceTagIdentification            sequenceTagIdentification            sequenceTagIdentification
interaction.xref                                    -                                    -                                    -
publication.id                               26929214                             26929214                             31046837
confidence                                       0.35                                 0.35                                 0.35
source.database                                IntAct                               IntAct                               IntAct
interaction.id   intact:EBI-16421609|imex:IM-26156-23 intact:EBI-16421284|imex:IM-26156-21 intact:EBI-21360986|imex:IM-26684-48
SYMBOL.A                                      KATNAL2                              KATNAL1                                LRRK2
ENTREZID.A                                      83473                                84056                               120892
GENEID.A                              ENSG00000167216                      ENSG00000102781                      ENSG00000188906
SYMBOL.B                                         CDK1                                 CDK1                                 PPIF
ENTREZID.B                                        983                                  983                                10105
GENEID.B                              ENSG00000170312                      ENSG00000170312                      ENSG00000108179
</pre>


# canonical identifiers

Here are some excerpts from Porras 2020, [Towards a unified open access dataset of molecular interactions, Nature Communications.](https://www.nature.com/articles/s41467-020-19942-z)

They make the case for using UniProtKB identifiers for proteins in the google data commons.  

I have condensed and rephrased some of their text for quicker reading.

  The consortium described:

   The IMEx Consortium is open to any group or resource inter- ested in curating
   physical molecular interactions, current members include IntAct, MINT,
   DIP, UniProt, MatrixDB, InnateDB, HPIDB, UCL Functional Gene
   Annotation team and IID. The consortium comprises the majority of the
   existing database resources who have agreed to collaborate on the curation
   of published, experimentally derived interaction data.  The IMEx Consortium
   members have agreed on a set of curation rules and map interaction data to a
   limited set of defined molecule identifiers to provide the user with a single
   and consistent dataset, with each interaction being assigned a unique and
   persistent identifier.


  uniprotkb ids apply at all levels of specificity (page 3):

     to all isoforms of a protein, collectively
     to any specific isoform
     to a post-translationally modified cleaved peptide chain
     coordinate-level mappings to amino acid sequence are available, 
        reprocessed at every 8-week curation run

  community consensus controlled vocabularies are used, extensions to which are negotiated over time
  
  regarding other molecules:

     Small molecule interactors, including carbohydrates and lipids, are mapped to 
     the ChEBI database
     Protein complexes to the Complex Portal
     mRNAs to Ensembl32 or ENA 
     ncRNAs to RNAcentral34 
     genes to Ensembl
