# OSINT - Find cell



## Challenge description:
![find_cell](https://user-images.githubusercontent.com/70543460/94421438-34568000-018e-11eb-944a-9a755a44134a.png)

## Challenge files:
[challenge.txt](https://github.com/Cyb3rDoctor/DarkCTF/files/5291566/challenge.txt)

<br/><br/>
## Solution:
<br/><br/>
First of all, you need to understand what are these values: (**eNB ID, MCC and MNC**)

<br/><br/>

And here is a table that gives a simple explanation about (**eNB ID, MCC and MNC**):
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94423524-7208d800-0191-11eb-9492-a8df2b38fa20.png)
<br/><br/>

<br/><br/>
...
<br/><br/>

In the challenge file, we have those 3 values:
<br/><br/>
310

410

81907
<br/><br/>
...
<br/><br/>

Now you need to identify those values **(I mean that you need to know which one is the eNB ID and which one is the MCC and which one is the MNC)**

<br/><br/>

To do that, search for a list of MCC and MNC, and here is a good one: (https://www.mcc-mnc.com/)
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94434597-ba7cc180-01a2-11eb-9707-d5a69a64ea40.png)
<br/><br/>

If you search for **310** in that site, you will find a lot of results, but if you search for **410**, you will find 8 results only, so it's better to check the fewer results:

<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94435019-455dbc00-01a3-11eb-8739-681c9213b4ae.png)
<br/><br/>

<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94435845-5529d000-01a4-11eb-971c-6f6c3e4f9f0a.png)
<br/><br/>

Nice, you now know that:

![image](https://user-images.githubusercontent.com/70543460/94436830-9a9acd00-01a5-11eb-9b70-b22607b82135.png)

<br/><br/>

Now you need to locate that cell tower...

<br/><br/>

One of the best sites to locate cell towers is (www.cellmapper.net)

<br/><br/>
You can search for a specific tower in cellmapper:
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94437804-f023a980-01a6-11eb-80c7-4f7e8b475145.png)
<br/><br/>

If you put the **eNB ID**	there, you will find a tower:
<br/><br/>
![image](https://user-images.githubusercontent.com/70543460/94438136-5e686c00-01a7-11eb-965c-cab2fdb8c70d.png)
<br/><br/>

![image](https://user-images.githubusercontent.com/70543460/94438243-83f57580-01a7-11eb-9d29-e5b03cac1e71.png)
<br/><br/>

**that's the tower you are looking for!**

(https://www.cellmapper.net/map?MCC=310&MNC=410&type=LTE&latitude=32.84644890905747&longitude=-24.554806096440018)

<br/><br/>

**darkCTF{32.8,-24.5}**
