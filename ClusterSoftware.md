# Cluster Software

## Info 

* [Wikipedia Article](https://en.wikipedia.org/wiki/Comparison_of_cluster_software) - Comparison of different cluster Software

* [Parallel Processing HOWTO](http://www.tldp.org/HOWTO/Parallel-Processing-HOWTO-3.html) - The Linux Documentation Project 

* [Survey of open source cluster management software](https://www.linux.com/news/survey-open-source-cluster-management-systems) - linux.com


## From Tony

This is resources I Recieved from Tony Travis at Minke Informatics

The software I mentioned is "oneSIS":

  http://onesis.org/

This is a way of sharing the root filesystem between multiple stateless
nodes and I used it on a 100+ node Beowulf at the Rowett Institute when
I worked there. It's not 'parallel processing' software. It's node
provisioning software. Most of the work we did on the Beowulf was
'embarrassingly' parallel in which the parallel execution threads don't
communicate, but we also ran some MPI parallel programs using Open MPI:

  https://www.open-mpi.org/

The distributed filesystem is called RozoFS and uses the Mojette
transform to create 'projections' of the data on each node that can't be
used independently. It's not encryption using a key. However, the result
is that individual 'projections' can't be used to recover any data. That
gives some level of security but its primary purpose is to provide
redundancy using a minimum of disk space and compute resource.

  http://rozosystems.com

The source code is GPL and freely available on GitHub:

  https://github.com/rozofs

Here is an example (in French) of RozoFS running on a cluster of RPi's:

  http://web.polytech.univ-nantes.fr/1400597692705/0/fiche___pagelibre

And a talk (in English) about RozoFS by one of the developers:

  http://acn2014.u-bordeaux.fr/files/SlidesACN/talk-parrein-acn-2014.pdf

