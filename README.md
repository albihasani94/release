## Maven Release Plugin

Release major and minor versions from the Maven relase plugin (by default, patch versions).

## Minor releases

```bash
mvn -B build-helper:parse-version release:prepare -DdevelopmentVersion=\${parsedVersion.majorVersion}.\${parsedVersion.nextMinorVersion}.0-SNAPSHOT
```

## Major releases

```bash
mvn -B build-helper:parse-version release:prepare -DdevelopmentVersion=\${parsedVersion.nextMajorVersion}.0.0-SNAPSHOT
```