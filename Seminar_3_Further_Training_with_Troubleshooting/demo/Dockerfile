#Use Ubuntu 22.04 as base
FROM ubuntu:22.04

#Install R
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y r-base libcurl4-openssl-dev libxml2-dev libssl-dev

#Install DeSeq2
RUN R -e "install.packages('BiocManager',dependencies=TRUE, repos='http://cran.rstudio.com/')"
RUN R -e "BiocManager::install('DESeq2')"
