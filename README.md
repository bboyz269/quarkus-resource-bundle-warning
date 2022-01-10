# Resource bundle warning in quarkus 2.6.1.Final

```
> ./gradlew clean assemble
Configuration on demand is an incubating feature.

> Task :quarkusGenerateCode
preparing quarkus application

> Task :quarkusBuild
building quarkus jar

Uber JAR strategy is used for native image source JAR generation on Windows. This is done for the time being to work around a current GraalVM limitation on Windows concerning the maximum command length (see https://github.com/oracle/graal/issues/2387).
Dependencies with duplicate files detected. The dependencies [javax.xml.bind:jaxb-api::jar:2.3.1[paths: ~\.gradle\caches\modules-2\files-2.1\javax.xml.bind\jaxb-api\2.3.1\8531ad5ac454cc2deb9d4d32c40c4d7451939b5d\jaxb-api-2.3.1.jar;], jakarta.xml.bind:jakarta.xml.bind-api::jar:2.3.3[paths: ~\.gradle\caches\modules-2\files-2.1\jakarta.xml.bind\jakarta.xml.bind-api\2.3.3\48e3b9cfc10752fba3521d6511f4165bea951801\jakarta.xml.bind-api-2.3.3.jar;], org.jboss.spec.javax.xml.bind:jboss-jaxb-api_2.3_spec::jar:2.0.0.Final[paths: ~\.gradle\caches\modules-2\files-2.1\org.jboss.spec.javax.xml.bind\jboss-jaxb-api_2.3_spec\2.0.0.Final\1d2b5404a556a4aeddde8a9676cec8ee01b4e0a0\jboss-jaxb-api_2.3_spec-2.0.0.Final.jar;]] contain duplicate files, e.g. javax/xml/bind/Validator.class
Dependencies with duplicate files detected. The dependencies [jakarta.el:jakarta.el-api::jar:3.0.3[paths: ~\.gradle\caches\modules-2\files-2.1\jakarta.el\jakarta.el-api\3.0.3\f311ab94bb1d4380690a53d737226a6b879dd4f1\jakarta.el-api-3.0.3.jar;], org.glassfish:jakarta.el::jar:3.0.4[paths: ~\.gradle\caches\modules-2\files-2.1\org.glassfish\jakarta.el\3.0.4\f48473482c0e3e714f87186d9305bcae30b7f5cb\jakarta.el-3.0.4.jar;]] contain duplicate files, e.g. javax/el/BeanELResolver$BPSoftReference.class
Dependencies with duplicate files detected. The dependencies [com.fasterxml.jackson.jaxrs:jackson-jaxrs-json-provider::jar:2.12.6[paths: ~\.gradle\caches\modules-2\files-2.1\com.fasterxml.jackson.jaxrs\jackson-jaxrs-json-provider\2.12.6\23debd9ac6b5530f3cce89d07a62a1acb0ec06a2\jackson-jaxrs-json-provider-2.12.6.jar;], com.fasterxml.jackson.module:jackson-module-jaxb-annotations::jar:2.12.6[paths: ~\.gradle\caches\modules-2\files-2.1\com.fasterxml.jackson.module\jackson-module-jaxb-annotations\2.12.6\a0bea2c6f98eb0dc24208b54a53da80ea459c156\jackson-module-jaxb-annotations-2.12.6.jar;], com.fasterxml.jackson.jaxrs:jackson-jaxrs-base::jar:2.12.6[paths: ~\.gradle\caches\modules-2\files-2.1\com.fasterxml.jackson.jaxrs\jackson-jaxrs-base\2.12.6\80379595faf4aa8a5ee1bc761e19b6467164de33\jackson-jaxrs-base-2.12.6.jar;]] contain duplicate files, e.g. META-INF/versions/11/module-info.class
Dependencies with duplicate files detected. The dependencies [javax.xml.bind:jaxb-api::jar:2.3.1[paths: ~\.gradle\caches\modules-2\files-2.1\javax.xml.bind\jaxb-api\2.3.1\8531ad5ac454cc2deb9d4d32c40c4d7451939b5d\jaxb-api-2.3.1.jar;], jakarta.xml.bind:jakarta.xml.bind-api::jar:2.3.3[paths: ~\.gradle\caches\modules-2\files-2.1\jakarta.xml.bind\jakarta.xml.bind-api\2.3.3\48e3b9cfc10752fba3521d6511f4165bea951801\jakarta.xml.bind-api-2.3.3.jar;]] contain duplicate files, e.g. META-INF/versions/9/javax/xml/bind/ModuleUtil.class
Dependencies with duplicate files detected. The dependencies [org.jetbrains.kotlin:kotlin-stdlib-jdk7::jar:1.6.10[paths: ~\.gradle\caches\modules-2\files-2.1\org.jetbrains.kotlin\kotlin-stdlib-jdk7\1.6.10\e1c380673654a089c4f0c9f83d0ddfdc1efdb498\kotlin-stdlib-jdk7-1.6.10.jar;], org.jetbrains.kotlin:kotlin-stdlib-jdk8::jar:1.6.10[paths: ~\.gradle\caches\modules-2\files-2.1\org.jetbrains.kotlin\kotlin-stdlib-jdk8\1.6.10\e80fe6ac3c3573a80305f5ec43f86b829e8ab53d\kotlin-stdlib-jdk8-1.6.10.jar;], org.jetbrains.kotlin:kotlin-reflect::jar:1.6.10[paths: ~\.gradle\caches\modules-2\files-2.1\org.jetbrains.kotlin\kotlin-reflect\1.6.10\1cbe9c92c12a94eea200d23c2bbaedaf3daf5132\kotlin-reflect-1.6.10.jar;], org.jetbrains.kotlin:kotlin-stdlib::jar:1.6.10[paths: ~\.gradle\caches\modules-2\files-2.1\org.jetbrains.kotlin\kotlin-stdlib\1.6.10\b8af3fe6f1ca88526914929add63cf5e7c5049af\kotlin-stdlib-1.6.10.jar;], net.bytebuddy:byte-buddy::jar:1.11.20[paths: ~\.gradle\caches\modules-2\files-2.1\net.bytebuddy\byte-buddy\1.11.20\340ea62787abad5682f17058e7c8928605e116d5\byte-buddy-1.11.20.jar;]] contain duplicate files, e.g. META-INF/versions/9/module-info.class
21.3-java11: Pulling from quarkus/ubi-quarkus-native-image
Digest: sha256:bd1b7e3e81b60239611eaae77aa390150b33da7fc4fb91028dee4034f1b5ab0e
Status: Image is up to date for quay.io/quarkus/ubi-quarkus-native-image:21.3-java11
quay.io/quarkus/ubi-quarkus-native-image:21.3-java11
[resource-bundle-warning-unspecified-runner:25]    classlist:  11,054.79 ms,  1.19 GB
[resource-bundle-warning-unspecified-runner:25]        (cap):     491.77 ms,  1.19 GB
[resource-bundle-warning-unspecified-runner:25]        setup:   2,653.46 ms,  1.19 GB
The bundle named: messages, has not been found. If the bundle is part of a module, verify the bundle name is a fully qualified class name. Otherwise verify the bundle path is accessible in the classpath.
06:37:15,808 INFO  [org.hib.val.int.uti.Version] HV000001: Hibernate Validator unspecified
06:37:16,137 INFO  [org.hib.Version] HHH000412: Hibernate ORM core version unspecified
06:37:16,151 INFO  [org.hib.ann.com.Version] HCANN000001: Hibernate Commons Annotations {5.1.2.Final}
06:37:16,247 INFO  [org.hib.dia.Dialect] HHH000400: Using dialect: org.hibernate.dialect.MySQL8Dialect
06:37:27,027 INFO  [org.jbo.threads] JBoss Threads version 3.4.2.Final
[resource-bundle-warning-unspecified-runner:25]     (clinit):     960.53 ms,  3.87 GB
[resource-bundle-warning-unspecified-runner:25]   (typeflow):   3,996.65 ms,  3.87 GB
[resource-bundle-warning-unspecified-runner:25]    (objects):  39,562.30 ms,  3.87 GB
[resource-bundle-warning-unspecified-runner:25]   (features):   6,763.73 ms,  3.87 GB
[resource-bundle-warning-unspecified-runner:25]     analysis:  53,650.43 ms,  3.87 GB
[resource-bundle-warning-unspecified-runner:25]     universe:   3,167.79 ms,  3.80 GB
[resource-bundle-warning-unspecified-runner:25]      (parse):   9,139.39 ms,  4.15 GB
[resource-bundle-warning-unspecified-runner:25]     (inline):  10,175.23 ms,  4.80 GB
[resource-bundle-warning-unspecified-runner:25]    (compile):  40,493.38 ms,  4.93 GB
[resource-bundle-warning-unspecified-runner:25]      compile:  63,298.90 ms,  4.93 GB
[resource-bundle-warning-unspecified-runner:25]        image:   4,437.45 ms,  4.93 GB
[resource-bundle-warning-unspecified-runner:25]        write:   1,320.97 ms,  4.93 GB
[resource-bundle-warning-unspecified-runner:25]      [total]: 140,249.48 ms,  4.93 GB
# Printing build artifacts to: /project/resource-bundle-warning-unspecified-runner.build_artifacts.txt

BUILD SUCCESSFUL in 2m 52s
7 actionable tasks: 7 executed
```