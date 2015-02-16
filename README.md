# DotCi-Fig-template
https://github.com/groupon/DotCi/pull/113 into its own plugin

Resources
 * https://wiki.jenkins-ci.org/display/JENKINS/Hosting+Plugins
 * https://groups.google.com/forum/#!topic/jenkinsci-dev/ftfibR23v5Y

If you have an account then publish latest [jenins nexus -SNAPSHOT](http://maven.jenkins-ci.org:8081/content/repositories/snapshots/com/groupon/jenkins-ci/plugins/DotCi) via
```
mvn deploy
```

or cut, tag, and bump the next [jenkins nexus releases](http://maven.jenkins-ci.org:8081/content/repositories/releases/com/groupon/jenkins-ci/plugins/DotCi) via
```
mvn release:prepare -e --batch-mode -Dresume=false -Darguments="-DskipTests"
mvn release:perform -e -Darguments="-DskipTests"
```
