#######################################################################################
## DO NOT EDIT THIS FILE! This file was automatically generated from the dockerfile. ##
## Run dynwrap:::.container_dockerfile_to_singularityrecipe() to update this file.   ##
#######################################################################################

Bootstrap: shub

From: dynverse/dynwrap:bioc

%labels
    version 0.1.1

%files
    . /code

%post
    chmod -R 755 '/code'
    apt-get install -y libudunits2-dev
    R -e 'devtools::install_github("farrellja/URD")'

%runscript
    exec Rscript /code/run.R

