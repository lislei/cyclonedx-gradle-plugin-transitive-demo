Demonstrates transitive dependencies in https://github.com/CycloneDX/cyclonedx-gradle-plugin

Se [SBOM produced with 1.7.0](moduleA/bom.1.7.0.xml) 
and [SBOM produced with 1.7.2](moduleA/bom.1.7.2.xml)


# Steps to reproduce:

$ ./gradlew cycloneDxBom -PbuildDir=testPluginVersion1.7.2

Then switch to plugin version 1.7.0 in [settings.gradle](settings.gradle) 

$ ./gradlew cycloneDxBom -PbuildDir=testPluginVersion1.7.0
