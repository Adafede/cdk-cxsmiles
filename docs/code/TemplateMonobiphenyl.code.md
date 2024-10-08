# TemplateMonobiphenyl.groovy
**Source code:**
```groovy
@Grab(group='org.openscience.cdk', module='cdk-smiles', version='2.9')
@Grab(group='org.openscience.cdk', module='cdk-silent', version='2.9')
@Grab(group='org.openscience.cdk', module='cdk-depict', version='2.9')

import org.openscience.cdk.smiles.SmilesParser;
import org.openscience.cdk.interfaces.*;
import org.openscience.cdk.silent.SilentChemObjectBuilder;
import org.openscience.cdk.isomorphism.UniversalIsomorphismTester;
import org.openscience.cdk.depict.DepictionGenerator;

sp = new SmilesParser(
  SilentChemObjectBuilder.getInstance()
)

mol = sp.parseSmiles(
  "Cl*.c1ccccc1-c1ccccc1 |m:1:3.4.5.6.7.8.9|"
)
new DepictionGenerator()
  .depict(mol)
  .writeTo("monochlorobiphenyl.svg");
```
**Output:**
```plain
```
