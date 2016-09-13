
TemplateNestedIncludeCurrentDirBugTest
=========================================

* run ` mvn clean test ` will see the bug!

* then modify CompiledIncludeNode will slove the problem:
  https://github.com/mvel/mvel/pull/69/files
  `
  wget https://raw.githubusercontent.com/qxo/mvel/e213dc83fbb615909ca81d2933497c655f673127/src/main/java/org/mvel2/templates/res/CompiledIncludeNode.java -O ./src/main/java/org/mvel2/templates/res/CompiledIncludeNode.java 
 mvn clean test  ==> OK
 `
