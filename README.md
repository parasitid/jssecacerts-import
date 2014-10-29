jssecacerts-import
==================

small tool too import ssl certs. backed up here for personal use.

the InstallCert.java file is downloaded from a link gathered on stackoverflow. cannot find neither promote the original author...
cannot remember the original license...

shame on me. send a pull request if ever someone claims paternity on this.


How to
======

run : 

$ java -cp . InstallCert [HOST]:[PORT] [CERT_FILENAME]

use, either, on your java app command line : 

$ java ... -Djavax.net.ssl.trustStore=[CERT_FILENAME]


or copy it to java-home/lib/security/jssecacerts : 

$ sudo cp [CERT_FILENAME] $JAVA_HOME/jre/lib/security/jssecacerts
