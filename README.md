# kg-imex
extract IMEx interactions into nodes and edges (entities and
relations), import variously

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
