Lab Report 3
---
Researching  Commands:  Find Command
---

#1) Finding a specific file with a specific name
---
Example 1
---
```
find ./written_2 -name Cuba-History.txt
./written_2/travel_guides/berlitz2/Cuba-History.txt
```
With this command, I am trying to find the Cuba-History.txt file. This command is useful because it returns the directory that the file is contained in, which is ./written_2/travel_guides/berlitz2/

My source for this example is from Week 4 of lab where I was encouraged to do a web search to learn about the -name option for find.


Example 2
---
```
find ./written_2 -name WhereToMalaysia.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
```
With this command, I am trying to find the WhereToMalaysia.txt file. This command is useful because it returns the directory ./written_2/travel_guides/berlitz1/

My source for this example is from Week 4 of lab where I was encouraged to do a web search to learn about the -name option for find.

#2) Finding files by approximate names
---

Example 3
---
```
jeffjimenez@Jeffs-MacBook-Pro docsearch % find ./written_2 -iname "*History*txt"
./written_2/travel_guides/berlitz1/HistoryJapan.txt
./written_2/travel_guides/berlitz1/HistoryJamaica.txt
./written_2/travel_guides/berlitz1/HistoryEgypt.txt
./written_2/travel_guides/berlitz1/HistoryIsrael.txt
./written_2/travel_guides/berlitz1/HistoryIndia.txt
./written_2/travel_guides/berlitz1/HistoryItaly.txt
./written_2/travel_guides/berlitz1/HistoryDublin.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt
./written_2/travel_guides/berlitz1/HistoryMallorca.txt
./written_2/travel_guides/berlitz1/HistoryJerusalem.txt
./written_2/travel_guides/berlitz1/HistoryMadrid.txt
./written_2/travel_guides/berlitz1/HistoryHongKong.txt
./written_2/travel_guides/berlitz1/HistoryIstanbul.txt
./written_2/travel_guides/berlitz1/HistoryLasVegas.txt
./written_2/travel_guides/berlitz1/HistoryGreek.txt
./written_2/travel_guides/berlitz1/HistoryHawaii.txt
./written_2/travel_guides/berlitz1/HistoryMadeira.txt
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt
./written_2/travel_guides/berlitz1/HistoryIbiza.txt
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
./written_2/travel_guides/berlitz1/HistoryFWI.txt
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
./written_2/travel_guides/berlitz2/Portugal-History.txt
./written_2/travel_guides/berlitz2/Costa-History.txt
./written_2/travel_guides/berlitz2/Barcelona-History.txt
./written_2/travel_guides/berlitz2/Berlin-History.txt
./written_2/travel_guides/berlitz2/Bali-History.txt
./written_2/travel_guides/berlitz2/Athens-History.txt
./written_2/travel_guides/berlitz2/California-History.txt
./written_2/travel_guides/berlitz2/Vallarta-History.txt
./written_2/travel_guides/berlitz2/Cancun-History.txt
./written_2/travel_guides/berlitz2/CostaBlanca-History.txt
./written_2/travel_guides/berlitz2/NewOrleans-History.txt
./written_2/travel_guides/berlitz2/PuertoRico-History.txt
./written_2/travel_guides/berlitz2/Nepal-History.txt
./written_2/travel_guides/berlitz2/China-History.txt
./written_2/travel_guides/berlitz2/Canada-History.txt
./written_2/travel_guides/berlitz2/Crete-History.txt
./written_2/travel_guides/berlitz2/Amsterdam-History.txt
./written_2/travel_guides/berlitz2/Beijing-History.txt
./written_2/travel_guides/berlitz2/Bermuda-history.txt
./written_2/travel_guides/berlitz2/CanaryIslands-History.txt
./written_2/travel_guides/berlitz2/Algarve-History.txt
./written_2/travel_guides/berlitz2/Poland-History.txt
./written_2/travel_guides/berlitz2/Budapest-History.txt
./written_2/travel_guides/berlitz2/Cuba-History.txt
./written_2/travel_guides/berlitz2/Bahamas-History.txt
jeffjimenez@Jeffs-MacBook-Pro docsearch % 
```
With this command, I am able to find files by approximate file name and it is a case in-sensitive search. In this case, it just finds all the txt files with History in the name. My source for this command is redhat.com/sysadmin/linux-find-command.


Example 4
---

```
find ./written_2 -iname "*hIstoRyHoNg*txt"
./written_2/travel_guides/berlitz1/HistoryHongKong.txt
```
With this command, I used -iname to find a file with the terms HistoryHong and it ignored the case sensitivity. It found an appropriate file. The source for this command is redhat.com/sysadmin/linux-find-command.

#3) Listing directories
---


Example 5
---
```
jeffjimenez@Jeffs-MacBook-Pro docsearch % find ./written_2 -type d
./written_2
./written_2/non-fiction
./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Berk
./written_2/non-fiction/OUP/Abernathy
./written_2/non-fiction/OUP/Rybczynski
./written_2/non-fiction/OUP/Kauffman
./written_2/non-fiction/OUP/Fletcher
./written_2/non-fiction/OUP/Castro
./written_2/travel_guides
./written_2/travel_guides/berlitz1
./written_2/travel_guides/berlitz2
```
With this command, I used -type d to list all of the directories in written_2. This is useful if I want to find all of the directories in a path. The source for this command was redhat.com/sysadmin/linux-find-command.
