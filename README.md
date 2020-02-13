# ICGC Score-client

ICGC score-client 2.2.1 Singularity recipe. Uses docker://alpine:3.10.3 as base image.

# Example

singularity run thakk-Score-client.sif sh -c 'export ACCESSTOKEN=this ; export STORAGE_PROFILE=that ; java -Xmx3G --illegal-access=deny -Dlogging.path=/tmp -Dspring.config.additional-location=/usr/local/score-client/conf/ -Dlogging.config=/usr/local/score-client/conf/logback.xml -cp /usr/local/score-client/lib/score-client.jar org.springframework.boot.loader.JarLauncher help'
