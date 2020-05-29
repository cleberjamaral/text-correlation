# text-correlation
Creates a correlation matrix among a set of given documents showing how strong is the relationship or similarity with them. It grab all documents from a specified folder using tensorflow universal sentence encoder creates vectors of them. 

By default, the folder with the documents is called `my_documents/` and the resulting files with all correlations will be placed on `correlation/` forlder. 

The csv output file `correlation/correlation.csv` can be imported in spreadsheet processors such as Microsoft Excel, Libre Office and Google Spreadsheets. The correlation near to 1 is maximum, close to zero is minimal, meaning no correlation. It is also suggested to use their tools for conditional formating to facilitate visualization.

By default, intermediary files greater than 500 kBytes are skipped.

Two other folders `correlation/texts/` and `correlation/vectors/` are created with intermediary files.

The original documents can be PDF, DOC and EPUB and others ([see tika documentation](https://tika.apache.org/0.9/formats.html))

Developed using Python 3.7.7
