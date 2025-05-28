# KGE_snomed_proc: code for training knowledge graph embeddings on the SNOMED ontology


Supplementary code for the paper *Measuring the effectiveness of knowledge graph embedding for biomedical ontologies: defining the distance between brocedures using SNOMED CT Embeddings*

This code converts the SNOMED ontology distribution files into usable triples, and trains KGE models.

0. You'll need a copy of the SNOMED ontology (UK editions are available for download from [NHS England](https://isd.digital.nhs.uk/trud/users/guest/filters/0/categories/26)) and the SNOMED transitive closure script (available from [SNOMED International](https://confluence.ihtsdotools.org/display/DOCRELFMT/Transitive+closure+file)).
1. `create_triples.ipynb` converts the SNOMED distribution files into triples for training.
2. `learn_embeddings.ipynb` uses [PyKeen](https://github.com/pykeen/pykeen) to train a KGE model using these triples.
