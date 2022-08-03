# matrisome-annotator

This webtool identifies ECM genes in datasets and annotates these genes according to matrisome divisions (core matrisome or matrisome-associated) and categories (ECM glycoproteins, collagens and proteoglycans, for core matrisome genes, ECM-affiliated, ECM regulators and secreted factors, for matrisome-associated genes) proposed by Naba and collaborators <a href="https://www.mcponline.org/article/S1535-9476(20)30479-5/fulltext">Naba et al, Mol Cell Prot, 2012</a>.

Input file requirements:

    The input file should be a comma separated value file (.csv).
    Entrez Gene Symbol of the input file should be in the second column and the header of the column should be "EntrezGeneSymbol" (no space).
    If you want to pipe MatrisomeAnnotator with MatrisomeAnalyzer to analyze mass spectrometry data, the following columns are mandatory: SampleName_Spectra, SampleName_PeptideAbundance, SampleName_UniquePeptides

Output file:

    The output file name will be annotations.filename.csv.
    The output file is a comma-separated text file that can be opened with excel.
    Matrisome division and category annotations will be in the first and second columns of the output file.
