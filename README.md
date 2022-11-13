# WEBFUSE V.1

Best Information Gathering Tool For Web Site Enuremation 2022

## Features

* Fuzz url set from an input file
* Concurrent relative path search
* Configurable number of fuzzing workers
* Fuzz CMS ==> Wordpress,Durpal,Joomla
* Generate reports of the valid paths
## Usage

~~~
$ python webfuse.py -h
Usage: webfuuse.py [options]

Options:
  -h, --help            show this help message and exit
  -q, --quiet           Silent mode ,only reports
  -u URL, --url=URL      URL of the Target
  -c CMS, --cms=CMS     scan CMS ==> wp ,dp
  -w WORDLIST, --wordlist=WORDLIST
                        Custom wordlist

~~~

Example:
* Fuzzing an url with default dictionary
~~~
python webfuse.py -u http://127.0.0.1 
~~~

* Fuzzing CMS (wp: in this exemple !)
~~~
python webfuse.py -u http://127.0.0.1 --cms wp 
~~~

* Fuzzing a custom Wordlist
~~~
python webfuse.py -u http://127.0.0.1 -w webdb/discovery/predictable-filepaths/php/PHP.txt
~~~




## How to install
##### Clone
 - Clone the repository with:
```sh
$ git clone https://github.com/Mrjaniya/webfuse.git
$ cd WebFuse
$ python webfuse.py
```
##### Dependencies
* Install the required dependencies with:
```bash
$ sudo pip install -r requirements.txt
```
## License
The MIT License (MIT) 2022
