### Generating POI Type Embeddings

To generate embeddings for types of points of interest (POI), you need to set up a PostgreSQL database and load the database instance from the following link: https://zenodo.org/doi/10.5281/zenodo.11094645.

Basic information about Austin and the urban zones of the city can be found in the Austin Data folder and is required to execute all notebooks.

To generate embeddings using GeoContext2Vec, you should execute the following notebooks:
- GeoContext2Vec-postgres.ipynb;
- GeoContext2Vec Word2Vec Training.ipynb (to generate Word2Vec embeddings);
- GeoContext2Vec_MLM_BERT_Finetuning_15Token-Pipeline.ipynb (to generate Distilbert embeddings).

To generate embeddings for the Shortest Path, you should execute the following notebooks in sequence:
- Zoning-Oriented Shortest Path Algorithm-postgres.ipynb;
- Shortest Path Corpus Generation-postgres.ipynb;
- Shortest Path Word2Vec Training.ipynb.

To generate embeddings for ITDL, you should execute the following notebooks in sequence:
- ITDL-postgres.ipynb;
- ITDL Word2Vec Training.ipynb.

Remember to update the login credentials for your database instance in each notebook.

Pre-calculated embeddings for all three methods can be found at the following link: https://drive.google.com/drive/folders/1mjXampBlO0fnfSCNq3F8cdqNZmnFkk1H?usp=sharing.