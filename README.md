# LanguageDatabase

## Target Domain
This project will focus on a database on world languages and immigration. It will have information on different features of world languages and on the estimated number of immigrants across different countries, allowing us to extract information on the relationship between immigration trends and the structure of the official languages of different countries. 


## Demo
I have used recordit to record the demo of the website:
#### Website Overview
<img src='http://g.recordit.co/hg0LKohZMQ.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### Filter languages
<img src='http://g.recordit.co/Ft9iNRpjbs.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### Group languages
<img src='http://g.recordit.co/bd7nzzEWbG.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### See language details
<img src='http://g.recordit.co/29jHGEBiSE.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### See location of language on map
<img src='http://g.recordit.co/Ra0r8ewyam.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### See attributes explanation
<img src='http://g.recordit.co/GQrcmaKelF.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### See Immigration data
<img src='http://g.recordit.co/NcOadRjfuu.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

#### Group Immigration data
<img src='http://g.recordit.co/O7lMRoOlmQ.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

## How to see the project
The project is included in this submission, in the folder “languages”. 
To run the code, you will have to make two modifications in languages/src/main/java/Server. Note that the place of those modifications are marked with "//TODO:"
1. In the sections marked by the comments, substitute the path to the appropriate CSV file as it appears on your computer. All the necessary CSV files are in src/main/resources/public/data inside the language foder. 
2. Uncomment the like populateTables() (there is a comment to indicate which like it is) and run Server
3. Go to localhost:7000 in your computer

Please see Demo section to understand how the website works


## How I loaded the data
I have used java scripts to load the different types of data. Those scripts are methods that can be found in the Server file. Moreover, I have used classes to represent the tables (see model folder), and classes to encapsulate methods to access the tables (see persistence folder). 
The sources of the data are:
 - Immigration data (by country of origin, country of destination, age, and sex) → https://www.un.org/en/development/desa/population/migration/data/estimates2/estimates15.asp
 - Language data (with genus, family, and country) → https://wals.info/languoid
 - Language consonant inventories → https://wals.info/feature/1A#2/19.3/152.9
 - Language vowel inventories → https://wals.info/feature/2A#2/19.3/152.9
 - Language consonant-vowel rations → https://wals.info/feature/3A#2/19.3/152.9 
 - Language uvular consonants → https://wals.info/feature/6A#2/19.3/152.9 
 - Language syllable structure → https://wals.info/feature/12A#2/19.3/152.9 
 - Number of genders → https://wals.info/feature/30A#2/26.7/149.1
 - Languages with sex-based and non-sex-based gender assignment → https://wals.info/feature/31A#2/26.7/149.1
 - Languages’ system of sex assignment → https://wals.info/feature/32A#2/26.7/149.1
 - Languages’ tones → https://wals.info/feature/13A#2/19.3/152.9 
 - Languages’ rhythm → https://wals.info/feature/17A#2/28.0/148.4
 - Languages’ order of subject, object and verb → https://wals.info/feature/81A#2/18.0/152.9
 - Languages’ absence of common consonants → https://wals.info/feature/18A#2/19.3/152.9 
 - Language’s presence of uncommon consonants → https://wals.info/feature/19A#2/12.9/116.0 

## Software Choice
I have used postgress for the database, and gradle to build the structure of the project. However, when running locally, the project uses mysql. Moreover, the project is set up to be deployed on heroku. 
The folder hierarchy and build files was created using Gradle

## Selling Points
 - Ability to visualize relationships between different languages
 - Ability to visualize relationships between country’s languages and immigration data
 - Google maps integration
 - Good use of object-oriented software engineering to store and retrieve data
 - Ability to filter queries using the same method no matter the number of parameters
 - Greater control of user input: users have to select options instead of typing a response, which increases security

## Database Definition Language

