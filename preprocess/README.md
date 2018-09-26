#Preprocess
# After convert the java-nlp-tookkit into jar, using the following code as
java -cp target/java-nlp-toolkit-0.1.3-SNAPSHOT.jar justhalf.nlp.reader.acereader.ACEReader -ace2004Dir ../../NLP/data/ACE2004/English -ace2005Dir ../../NLP/data/ACE2005/English -ace2004OutputDir ace2004_out -ace2005OutputDir ace2005_out -dataSplit 0.9,0.1,0.1 -printEntities -tokenizer stanford -posTagger stanford -splitter stanford -shuffle -seed 31

#random split seed set as 31 in the jave preprocessing code
# the data format is as:
# Line1: "we have a major development to report tonight involving the crash of that singapore airlines 747 in taiwan this week ."
# Line2: "PRP VBP DT JJ NN TO VB NN VBG DT NN IN DT NN NNS CD IN NN DT NN ."
# Line3: "0,1,0,1 ORG|12,16,15,16 VEH|13,15,13,15 ORG|17,18,17,18 GPE"
# Line4: "\n"

