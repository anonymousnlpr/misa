<h1> Multilingual IsA (MIsA)</h1>  
This is the source code of the project MIsA:  http://web.informatik.uni-mannheim.de/misa/
<h2>INSTALL</h2>  
1) download install tt4j from https://reckart.github.io/tt4j/ and copy "org.annolab.tt4j-1.2.1.jar" into the project lib folder.
2) edit the file "data/properties" and specify the following properties:  
  
  treetaggerhome	<path of your "TreeTagger" installation folder>  
  treetaggerlib	<path of your "TreeTagger/lib" folder>  
  
3) download and install stanford-corenlp v. 3.4.1 from https://stanfordnlp.github.io/CoreNLP/download.html and copy "stanford-corenlp-3.4.1.jar" into the project "lib" folder.
4) download from https://nlp.stanford.edu/software/tagger.shtml#Download all the following language models:  
english-left3words-distsim.tagger        french.tagger        german-fast-caseless.tagger        german-fast.tagger        german-hgc.tagger        german-ud.tagger        spanish-distsim.tagger        spanish.tagger
english-left3words-distsim.tagger.props  french.tagger.props  german-fast-caseless.tagger.props  german-fast.tagger.props  german-hgc.tagger.props  german-ud.tagger.props  spanish-distsim.tagger.props  spanish.tagger.props
and copy them to the project "models" folder.

<h2>HOW TO RUN:</h2>
compile the project and run from command line: 
java -cp ./lib:./lib/* de.unima.multilingual.MIsA <language> <inputFolder> <outputFile>

where:
<language> is one from DE,EN,ES,FR,IT and NL;
<inputFolder> is the folder containing all the ".txt" files to be processed;
<outputFile> is the name of the otput file thaht will contatins  the extracted tuples. 

Our source code is licensed under a Creative Commons Attribution 4.0 International (CC BY-NC 4.0) License: https://creativecommons.org/licenses/by-nc/4.0/.
For the Stanford Log-linear Part-Of-Speech Tagger and for the TreeTagger please refer to the corresponding licenses.

