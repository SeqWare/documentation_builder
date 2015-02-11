This creates and updates documentation at seqware.github.com 

Assumes that seqware\_whitestar has already been built. 

---------------------------------------------------------------

For developers

1. Add an appropriate private key at private\_key.pem

2. Assuming docker is installed properly, build image with 

        docker build  -t seqware_1.1.0-alpha.6_docs .

3. Run container and build our docs with the following 
 
        docker run --rm -h master -t -i seqware_1.1.0-alpha.6_docs

