<h1>SQL-Injection-Attack(pentest-report)</h1>



<h2>In this security assessment, I found a serious SQL injection in THE client web app. Using the inspector tool in the web browser, I exploited this flaw to access sensitive info left unprotected by the app. This kind of flaw is common and happens when the app doesn't check user input properly.
To recreate this, I looked at the app's code using a tool in the browser and found a part that looked like this: <option value="1">1</option>. I then used a trick to add my own code: <option value="1 OR 1=1#">1</option>. This made the app show info it shouldn't. To fix this, developers should check user input better and use special techniques to prevent these kinds of problems. #SQLInjection #WebSecurity <br />


<h2>Tools used:

- <b>Webb Inspector</b> 

<h2>Report Walkthrough:</h2>

<p align="center">
Brute force report introduction: <br/>
<img src="https://i.ibb.co/7Wj8xzh/Picture-SQL1.jpg" alt="Picture-SQL1"/>
<br />
<br />
Closer look: <br/>
<br />
<br /> 
<img src="https://i.ibb.co/5YXXCXV/Screenshot-677.png" alt="Screenshot-677"/>
<br />
<br />
Hidden information exposed after the attack:  <br/>
<br />
<br /> 
<img src="https://i.ibb.co/pK8VQ97/Picture-SQL2.jpg" alt="Picture-SQL2"/>
<br />
<br />





<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
