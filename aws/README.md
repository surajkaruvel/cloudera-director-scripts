# AWS RHEL 7.2 with Security Integration - Authentication and Authorization

This is a Director configuration that is intended to be a guide for integration Authentication and Authorization on the AWS cloud.  This will help automate the build process of a CDH cluster in the AWS cloud and assumes that a Cloudera Director server is already up and running.

When modifying these scripts the REPLACE_ME tag has been used so it is best to find and replace with the appropriate values.

This script requires many security and networking pieces to be ready to go.  It is assumed that AD is used as the KDC and permissions are pre-built based on the parameters passed in the script.


## Script Order

0. Create 1 VM for the Director Server and have the server up and running.
1. director.sh
  * Builds a complete cluster with Authentication and Authorization configured.
