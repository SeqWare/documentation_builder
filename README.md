This creates and updates documentation at seqware.github.com 

Assumes that seqware\_whitestar has already been built. 

---------------------------------------------------------------

For developers:

1. Build a host that has Docker installed, we normally use a Ubuntu host. 
2. Check out this repo 
3. Add an appropriate private key at private\_key.pem (This is a private key for the seqware-jenkins account on Github that is used to check in documents. Do not use a passphrase.)

4. Assuming docker is installed properly, build image with 

        docker build  -t seqware_1.1.0-alpha.6_docs .

5. Run container and build our docs with the following (this can be done via jenkins)
 
        docker run --rm -h master -t -i seqware_1.1.0-alpha.6_docs

