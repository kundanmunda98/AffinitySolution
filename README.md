# Degree of Profanity for Racial Slurs

This is a small python program that tags a profanity degree ( "HIGH" or "LOW" ) based on the slur words present in a tweet/sentence.
[credits](#credits-1)
## Project Tree:
```bash
|-- Data
|   |-- racial_slur_collection
|   |      |--ethnic_slurs.csv
|   |-- tweets_data.csv
|-- output_result.csv
|-- profanity_degree.py
```

* ### profanity_degree.py :
  * This program takes an input file e.g tweets_data.csv as a command line argument
  * And using the profanityfilter library methods, it tags a profanity-degree of either "HIGH" or "LOW" to the tweets/sentences based on the presence of slur words.
  * The tagged tweets/sentence is next written in a output_result.csv file.

>e.g : In the command line
>for input_file in the root folder
```
python.exe profanity_degree.py input_file_name.csv
```
>for input_file in the other folder, input the whole path
```
python.exe profanity_degree.py D:/folder1/folder2/input_file_name.csv
```
>for folder names with spaces use double quotes ''
```
python.exe profanity_degree.py 'D:/folder 1/folder 2/input_file_name.csv'
```

* ### Data : ethnic_slurs.csv
  * This is scraped dataset of ethnic slur terms from the Wikipedia website : https://en.wikipedia.org/wiki/List_of_ethnic_slurs.
  * One can personalise the dataset by adding custom slur/other words collection.


### Credits 1
This project is built on the library [profanityfilter](https://github.com/areebbeigh/profanityfilter) by [@areebbeigh](https://github.com/areebbeigh)

