# java-word-count-beam

## Ajay Kumar Reddy Arram

### The steps need to be followed to run the code and get an ouput file on word count


PS> mvn archetype:generate -D archetypeGroupId=org.apache.beam -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples -D archetypeVersion=2.36.0 -D groupId=org.example -D artifactId=word-count-beam -D version="0.1" -D package=org.apache.beam.examples -D interactiveMode=false

cd .\word-count-beam

dir .\src\main\java\org\apache\beam\examples

In the word-count-beam directory, create a file called sample.txt.
Run WordCount Using Maven
PS> mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount ` -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
