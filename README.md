# DotCi-Fig-template
https://github.com/groupon/DotCi/pull/113 into its own plugin

Resources
 * https://wiki.jenkins-ci.org/display/JENKINS/Hosting+Plugins
 * https://groups.google.com/forum/#!topic/jenkinsci-dev/ftfibR23v5Y

If you have an account then publish latest [jenins nexus snapshot](http://maven.jenkins-ci.org:8081/content/repositories/snapshots/com/groupon/jenkins-ci/plugins/DotCi-Fig-template) via
```
mvn deploy
```

and you'll need to manually cut, tag, bump the pom.xml to the next [jenkins nexus releases](http://maven.jenkins-ci.org:8081/content/repositories/releases/com/groupon/jenkins-ci/plugins/DotCi-Fig-template) then ```mvn deploy`` because the following appears to be broken
```
mvn release:prepare
mvn release:perform
```
