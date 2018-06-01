FROM jetbrains/teamcity-server

#add certificates for docker registry by adding certificates to JVM
COPY sampleCert.crt /sampleCert.crt
RUN /usr/lib/jvm/oracle-jdk/jre/bin/keytool -importcert -file /sampleCert.crt -keystore /usr/lib/jvm/oracle-jdk/jre/lib/security/cacerts -noprompt -storepass changeit
