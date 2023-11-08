# Search_engine_text_image
This project involves the design, development and evaluation of a multi-purpose system that includes a text search engine and an image search engine.The aim of this project is to provide users with a user-friendly interface to search for images based on their textual content, or to upload an image and find similar images in a database of images from Flickr. The system integrates technologies such as Elasticsearch, Streamlit and a pre-trained EfficientNet model to extract visual characteristics.
# Interface
![image](https://github.com/yomna99/moteur_de_recherche/assets/114284730/c24cd051-d88a-43ae-b8d6-dadb8ec0fd45)
# Prerequisites
first you should install: 
  * Elasticsearch 8.10.4 (https://www.elastic.co/fr/downloads/past-releases/elasticsearch-8-10-4)
  * Logstash 8.10.4 (https://www.elastic.co/fr/downloads/past-releases/logstash-8-10-4)
  * this is the link of the csv file of my flicker dataset
# How to run the project
* Clone the repository
* firstly you should load the tags of your flicker dataset into the elasticsearch index using Logstash and the file "phtotos_flickr_conf_73.conf"
* you can check if you had created the index successfully by running (http://localhost:9200/_cat/indices?)
* Create another index for the image search engine by runing the file "create_index"
* extract feature vectors by runing the file "search1.py"
* load the feature vectors into your image search index by runing the file "index_image.py"
* run the streamlit app using this command "streamlit run app.py"

