# Digital Innovation One

Code created to be utilized on Digital Innovation One platform.

<p align="center"><img src="./DIO.png" width="500"></p>

## Desafio GCP Dataproc

This code challenge is part of the course on Digital Innovation One platform:

__*Creating a fully managed Hadoop Ecosystem with Google Cloud Platform*__

Authored and proposed by Marcelo Marques (Cloud Architect at GFT Brasil):
https://github.com/marcelomarques05

Challenge accepted and submitted by Luis Vieira (Sr. Escalation Engineer, Tier 4 at Poly Inc.)
https://github.com/gutovieira

The objective of this challenge consists in executing some data processing using the product Dataproc on Google Cloud Platform. This procedure should perform a word count in a book (txt format file) and return the max number of occurrences each word appears in it.

---

### Steps

1. Create a bucket under Cloud Storage
1. Update the file ```contador.py``` replacing ```{SEU_BUCKET}``` with the name of the Bucket created on step 1.
1. Upload the files ```contador.py``` and ```livro.txt``` into the bucket (instructions below, if needed).
    - https://cloud.google.com/storage/docs/uploading-objects

1. Use the code in a Dataproc cluster, running a PySpark type job calling ```gs://{SEU_BUCKET}/contador.py```
1. The job will create a folder in the bucket named as ```resultado```. Within the folder, you will see the file ```part-00000``` that contains word list with the max number of occurrences in the entire book.

### Delivery

1. Create a GitHub repository.
2. Create a new file named ```resultado.txt```, add the top 10 words with more occurrences in the book, according to the job result.
3. Add the files ```resultado.txt``` and ```part-00000``` into your GitHub repository and submit your project via Digital Innovation One platform.

---

