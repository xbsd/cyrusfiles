# cyrusfiles
Cyrus of Artamene Files

Files for Artamène ou le Grand Cyrus (English: Artamène, or Cyrus the Great). The site (www.artamene.org) was taken offline and the text is now only available via the Wayback Machine (https://web.archive.org/web/20050511235238/http://www.artamene.org/)

The text was used in order to perform wordcount testing, one of the exercises in the following book:

Practical Big Data Analytics: Hands-on techniques to implement enterprise analytics and machine learning using Hadoop, Spark, NoSQL and R

Paperback: 412 pages
Publisher: Packt Publishing (January 15, 2018)
Language: English
ISBN-10: 1783554398
ISBN-13: 978-1783554393
Product Dimensions: 7.5 x 0.9 x 9.2 inches

The files have been added in the repository.

Simply change the URL as shown below in the file `getCyrusFiles.sh` as descriped on Pg. 83 of the text.

```The steps are as follows:
1. Create getCyrusFiles.sh - this script will be used to retrieve the data from the web:
            [cloudera@quickstart ~]$ mkdir cyrus
            [cloudera@quickstart ~]$ vi getCyrusFiles.sh
            [cloudera@quickstart ~]$ cat getCyrusFiles.sh
            for i in `seq 10`
            do
            # curl www.artamene.org/documents/cyrus$i.txt -o cyrus$i.txt (# Comments out this line)
            curl https://raw.githubusercontent.com/xbsd/cyrusfiles/master/cyrus$i.txt -o cyrus$i.txt
            done```
