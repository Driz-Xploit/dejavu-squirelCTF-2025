# dejavu-squirelCTF-2025 (Under-Contruction)
<img src='https://ctf.squ1rrel.dev/assets/squ1rrel_logo.webp' width='500' height='150'>

<hr>
<br>

## 1. Information Gathering (How does it work?)
<br>

### 1.1 Security and functions address analysis
<hr>
<img src='img/1.png' width='600' height='750'>
<hr><br>

As you can see, this binary has a protection by NX (Not Executable) and the function address is:
<ol>
<li>
  <strong>main: <italic>0x004012ec</italic></strong>
</li>
<li>
  <strong>win: <italic>0x004011f6</italic></strong>
</li>
</ol>
<br>

### 1.2 logic of functions analiysis
<hr>

#### Main function:
<img src='img/2.png' width='950' height='1000'>
<hr>

#### Win function:
<img src='img/3.png' width='950' height='1000'>
<hr><br>
The main function calls a <gets> that receives input from user and win function calls a <fopen> and <printf> that show the flag
