# OSINT - Dark Social Web



## Challenge description:
![dark_social_web](https://user-images.githubusercontent.com/70543460/94454704-dd1ad480-01ba-11eb-8193-c5f2eb87039d.png)


<br/><br/>
## Solution:
<br/><br/>

There is a username in the challenge description (**0xDarkArmy**)...

I checked all the social media sites for that username, and I found an interesting thing in **Reddit**!

<br/><br/>

(https://www.reddit.com/user/0xDarkArmy/)

![image](https://user-images.githubusercontent.com/70543460/94455063-54506880-01bb-11eb-8858-0dd643ca1fd8.png)

<br/><br/>

I scanned that QR code and I got this link: (https://qrgo.page.link/zCLGd), which redirects to this link: (http://cwpi3mxjk7toz7i4.onion/)

<br/><br/>

For those who don't know what is **.onion**:

![image](https://user-images.githubusercontent.com/70543460/94455578-e9536180-01bb-11eb-9b41-c27b32140399.png)

<br/><br/>

I opened TOR browser, then I opened that link and I got this website:

<br/><br/>
![site](https://user-images.githubusercontent.com/70543460/94456114-19026980-01bc-11eb-8ab9-95f62c7ce80f.png)
<br/><br/>

<br/><br/>

**I checked the source code, the CSS files and the JS files and I didn't find anything special...**

<br/><br/>

![source](https://user-images.githubusercontent.com/70543460/94456729-48b17180-01bc-11eb-8c68-3299a9fce1d3.png)
![source2](https://user-images.githubusercontent.com/70543460/94456731-49e29e80-01bc-11eb-82ca-8a487e9dbf95.png)


<br/><br/>

Then I checked **/robots.txt** and I found a part of the flag:

<br/><br/>
![robots txt](https://user-images.githubusercontent.com/70543460/94456993-a645be00-01bc-11eb-8e63-4f56f1c85ec6.png)
<br/><br/>

<br/><br/>

To make a long story short 😅, I found the other part of the flag in a header of a GET request:

![request](https://user-images.githubusercontent.com/70543460/94457570-6a5f2880-01bd-11eb-9e74-015ed3f1151d.png)

<br/><br/>

**darkctf{S0c1a1_D04k_w3b_051n7}**
