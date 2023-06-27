### Data
Here you can find all the relevant dataset used in this thesis:
1) [ParlVote corpus](https://data.mendeley.com/datasets/czjfwgs9tm/1)
2) [ParlaMint 2.1 corpora](https://www.clarin.si/repository/xmlui/handle/11356/1432)
3) [Translated Parlamint corpora](https://github.com/TajaKuzman/Parlamint-translation/tree/master)
4) [ParlGov](https://www.parlgov.org/data-info/)

### Automatic Labelling Experiments
To run the experiments, please download the 'parlvote_concat.csv' file from [Mendeley](https://data.mendeley.com/datasets/czjfwgs9tm/1). After, download the 'Automatic labelling experiments.ipynb' file and place this in the same folder as the 'parlvote_concat.csv' file. If you have Python installed, you should then be abel to run the notebook. 

### Parliamentary Search Engine
Due to file size restrictions on GitHub, the relevant files for the search engine can be downloaded from [Google Drive](). Here, you can find the notebook 'Search Engine.ipynb' which contains the preprocessing and the process fo loading the data into Elasticsearch. However, to experiment with the search engine, it is easier to just download the Elasticsearch and Kibana folder from the Google Drive. After you have downloaded these folders, you can open your command prompt. First, move to the Elasticsearch/bin folder and enter the command 'elasticsearch.bat'. This will start Elasticsearch. Second, move to the Kibana/bin folder and enter the command 'kibana.bat'. This will start Kibana.  

After, open your browser (preferably Google Chrome) and go to https://localhost:9200/ to check if Elasticsearch is running. You will be asked to login, for this you can use the following credentials: username = 'elastic' | password = 'fPWCz0GV61BwO22DjB0b'. If the tagline displays 'You Know, For Search', then Elasticsearch is running correctly. Now, you can navigate to http://localhost:5601/app/home#/ to open Kibana. You can use the same credentials to login. After, you can navigate to two different dashboards in the top left corner. The ‘Final Search Engine’ dashboard is the search engine evaluated by the political scientists. The ‘Sentiment Comparison’ dashboard is the environment that has been used for comparing negativity between the parliaments of different European countries. If you do not see any visualisations, make sure you have adjusted the time period in the top right corner to the correct interval. 
