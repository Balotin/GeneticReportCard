# GeneticReportCard
Java code for producing Genetic Report Cards from P. falciparum BAM files

Documentation is available on the wiki page at https://github.com/malariagen/GeneticReportCard/wiki


# Clone the repository
git clone https://github.com/Balotin/GeneticReportCard.git
# Building the tools
cd AnalysisCommon
ant build

cd ../SequencingReadsAnalysis
ant build

# Define project directories 
export GRCC=/home/student/GeneticReportCard/AnalysisCommon
export GRCA=/home/student/GeneticReportCard/SequencingReadsAnalysis

# Set the CLASSPATH variable by concatenating required paths and jar files
export CLASSPATH=$GRCA/bin:$GRCC/bin:\
$GRCC/lib/commons-logging-1.1.1.jar:\
$GRCA/lib/apache-ant-1.8.2-bzip2.jar:\
$GRCA/lib/commons-compress-1.4.1.jar:\
$GRCA/lib/commons-jexl-2.1.1.jar:\
$GRCA/lib/htsjdk-2.1.0.jar:\
$GRCA/lib/ngs-java-1.2.2.jar:\
$GRCA/lib/snappy-java-1.0.3-rc3.jar:\
$GRCA/lib/xz-1.5.jar
