# Load Historical Australian Stock Prices Into Elasticsearch From CSV (using logstash)

Usage: 
Basically just called the script asx-stock-prices.sh and pass your elastic search hostname. E.g.

./asx-stock-prices.sh localhost

Data file is stored on dropbox and is downloaded by the script - please note the dataset is pretty big i.e. around 6 million rows so you may want to look at one of the other examples first . 

The logstash configuration file leverages the translate filter plugin to emblish events with information from a reference data CSV (https://github.com/logstash-plugins/logstash-filter-translate).
