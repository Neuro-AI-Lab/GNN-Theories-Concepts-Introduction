๋ณธ๋ฌธ : (https://velog.io/@kimdyun/Inductive-Transductive-Learning-%EC%B0%A8%EC%9D%B4%EC%A0%90)

### ๐ค ์ด๋ฒ ์๊ฐ์๋ Inductive Learning๊ณผ Transductive Learning์ ์ฐจ์ด์ ์ ๋ํด ์๊ฐ๋ฅผ ํด๋ณด๋ ค๊ณ  ํ๋ค.

Inductive Learning์ ์ง์ญํ๋ฉด ๊ท๋ฉ์  ํ์ต, Transductive Learning์ ... ์ง์ญ์กฐ์ฐจ ์ ๋งคํ๋ค.
๋จ์ด๋ง ๋ณด๊ณ  ๊ทธ ๊ฐ๋์ ์ ์ถํ๊ธฐ ์ด๋ ค์ด ์ด ๋ ๋จ์ด๋ ์๋ง ์์ด ์์๋ก ๋ ์ฑ์ด๋ ์๋ฃ๋ก ๋จธ์  ๋ฌ๋์ ๊ณต๋ถํ๋ค๋ณด๋ฉด ์์ฃผ ๋ณด์์ ๊ฒ์ด๋ค. ํ์ง๋ง ๋ผ๋ฌธ์์ ์กฐ์ฐจ๋ ๋ ๊ฐ๋์ ์ง๊ด์ ์ผ๋ก ์ค๋ชํด์ฃผ์ง ์๋๋ค.
๊ทธ๋์ ์ด๋ฒ ์๊ฐ์๋ ๋จธ์ ๋ฌ๋์์ ๋ ํ์ต ๋ฐฉ์์ ๋ํ ๊ฐ๋๊ณผ ๊ทธ ์ฐจ์ด์ ๋ํด ์ฝ๊ฒ ์๊ฐํด๋ณด๋ ค๊ณ  ํ๋ค.

๐ฌ ๊ธ ์ฝ๊ธฐ ๊ท์ฐฎ์๋ ์๋ 3๋ฒ์๋ ๊ทธ๋ฆผ ์์๊ฐ ๋์ค๋... ํ์ดํ... ๐

<br><br>
### ๐ ๋จ์ด ์ ์ (Referenced by Wikipedia)
### &nbsp; ๐ _Transduction_
> In logic, statistical inference, and supervised learning, _**Transduction**_ is reasoning from observed specific (training) cases to specific (test) cases.

### &nbsp; ๐ _Induction_
> In contrast, _**induction**_ _**is reasoning**_ from observed training cases to _**general rules**_, which are then applied to the test cases.

&nbsp; Inductive Learning์ ์ ํต์ ์ธ ์ง๋ ํ์ต (supervised learning)์ ๋ฐฉ์๊ณผ ๊ฐ๋ค. ๊ทธ ๋ฐฉ์์ ๋ณด์๋ฉด, ์ฐ์  ๋จธ์ ๋ฌ๋ ๋ชจ๋ธ์ ์ค๊ณํ ๋ค **์ค์ง training dataset**๋ง์ ์ฌ์ฉํ์ฌ ๋ถ๋ฅ ํน์ ํ๊ท๋ฅผ ์ํ ๊ท์น(rule)์ ์ค์ค๋ก ์ถ๋ก ํ๋ค. ์ฆ, ๊ด์ธก๋ (observed) ๋ฐ์ดํฐ๋ training dataset ๋ฟ์ด๋ฉฐ ์ง๋ ํ์ต์ ํตํด training dataset ๋ถํฌ์ ์ต์ ํ๋ ๋ชจ๋ธ ํ๋ผ๋ฏธํฐ๋ฅผ ๊ณ์ฐํ๋ค. ์ดํ ๋ชจ๋ธ ํ์ต์ด ๋๋ ๋ค unlabeled testing dataset์ label์ ์ถ๋ก ํ๋ ์ด ์ง๋ ํ์ต ๋ฐฉ์์ด ๋ฐ๋ก ๋ํ์ ์ธ Inductive Learning์ ๊ฐ๋์ด๋ค.

&nbsp; ์ด์ ๋ฐํด Transductive Learning์ ํ์ต ์ ์ฌ์ ์ ๋ฏธ๋ฆฌ **training dataset** ๋ฟ๋ง ์๋๋ผ **testing dataset**๋ ์๊ณ  ์๋ (๊ด์ธกํ) ์ํ์ด๋ฉฐ, testing dataset์ label์ ์์ง ๋ชปํ์ง๋ง ํ์ต์ด ์งํ๋๋ ๋์ labeled data (training dataset)์ ํน์ง ๊ณต์  ํน์ ์ ํ, ๋ฐ์ดํฐ๊ฐ์ ์ฐ๊ด์ฑ, ํน์ง ํจํด ๋ฑ ์ถ๊ฐ์ ์ธ ์ ๋ณด๋ฅผ ํ์ฉํจ์ผ๋ก์จ testing dataset์ label์ ์ถ๋ก ํ๋ค.

 &nbsp; ๋ํ์ ์ธ Transductive Learning ๊ธฐ๋ฒ์ผ๋ก๋ **transductive SVM (TSVM)**, **graph-based label propagation algorithm (LPA)**, ๊ทธ๋ฆฌ๊ณ  **node-classification ๊ธฐ๋ฐ graph convolutional neural networks (GCN)์ feature propagation ๊ธฐ๋ฒ** ๋ฑ์ด ์๋ค. ์ฐธ๊ณ ๋ก ์ค์ง๋ ํ์ต (Semi-supervised Learning)๊ณผ ๋น์ทํ ์ ์ด ๋ง๋ค.
 
 <br><br>
 ### ๐ ์ฐจ์ด์  ์ ๋ฆฌ
 
&nbsp; ์ด์  ์ด๋์ ๋ Transductive Learning๊ณผ Inductive Learning์ ์ ์์ ๋ํด ์ดํด๊ฐ ๋์๋ค๋ฉด ๋ ํ์ต ๊ธฐ๋ฒ์ ์ฐจ์ด์ ์ ๋ํด ์์ธํ ์ ํ์๊ฐ ์๋ค.

&nbsp; ๋ค์ ํ๋ฒ ๊ฐ์กฐํ์๋ฉด, ๋ ๊ธฐ๋ฒ์ ๊ฐ์ฅ ํฐ ์ฐจ์ด๋ Transductive Learning์์ ๋ชจ๋ธ ํ์ต ์ training set๊ณผ testing set ๋ ๋ค ์ฌ์ฉํ๋ ๋ฐ๋ฉด, Inductive Leaning์์๋ ๋ชจ๋ธ ํ์ต ์ training set๋ง ์ฌ์ฉํ๋ฉฐ, ์ดํ์ ์ฐ๋ฆฌ๊ฐ ๊ด์ธกํ ์  ์๋ ์๋ก์ด testing dataset์ ํ์ต๋ ๋ชจ๋ธ์ ์ ์ฉํ๋ค.

&nbsp; Inductive Learning์์๋ ์๋ก์ด ๋ฐ์ดํฐ์ label์ ์ถ๋ก ํ  ์ ์๋ ๋ชจ๋ธ (predictive model)์ ์์ฑํ๋ฉฐ, ์ด ๋ ์๋ก์ด ๋ฐ์ดํฐ๋ฅผ ๊ด์ธกํ๋ค๊ณ  ํด์ ํ์ต ์์ฒด๋ฅผ ๊ผญ ๋ค์ ํ  ํ์๋ ์๋ค. ์๋ํ๋ฉด, ์ด๋ฏธ ํ์ต๋ ๋ชจ๋ธ์ ์๋ก์ด ๋ฐ์ดํฐ์ ์ ์ฉํ์ฌ ๊ทธ ๋ฐ์ดํฐ์ label์ ์ถ๋ก ํ๋ฉด ๋๊ธฐ ๋๋ฌธ์ด๋ค.

### &nbsp; ๐ฅ ์ฃผ์ ์ฌํญ
> &nbsp; ๋ถ๋ฅ ๋ฌธ์ ๋ฅผ ์๋ก ๋ค์๋ฉด, ํ์ต ์ ์ฌ์ฉํ ๋ฐ์ดํฐ๊ฐ ๊ฐ์ ๊ณ ์์ด ๋ฟ์ด์๊ณ , ์๋ก ๊ด์ธก๋ ๋ฐ์ดํฐ๊ฐ ๊ฐ ๋๋ ๊ณ ์์ด์ ๊ด๋ จ๋ ๋ฐ์ดํฐ์ผ ๋ ํ์ต์ ๋ค์ ํ  ํ์๊ฐ ์๋ค๋ ๊ฒ์ด๋ค. ๋ง์ฝ ์๋ก ๊ด์ธกํ ๋ฐ์ดํฐ๊ฐ ์ฝ๋ผ๋ฆฌ ๊ด๋ จ ๋ฐ์ดํฐ์ด๊ณ  ์ฝ๋ผ๋ฆฌ๋ ๋ถ๋ฅํ  ์ ์์ผ๋ฉด ์ข๊ฒ ๋ค๋ผ๊ณ  ํ๋ค๋ฉด ์ฝ๋ผ๋ฆฌ ๊ด๋ จ ๋ฐ์ดํฐ์ ํจ๊ป ๋ค์ ๋ชจ๋ธ์ ํ์ตํด์ผ ํ๋๊ฑด ๋น์ฐํ๋ค.

&nbsp; ๋ฐ๋ฉด **Transductive Learning์ predictive model์ ์์ฑํ์ง ์๋๋ค.** ๋ง์ฝ ์๋ก์ด ๋ฐ์ดํฐ๊ฐ ๊ด์ธก์ด ๋๋ค๋ฉด ํด๋น ๋ฐ์ดํฐ์ label์ ์์ธกํ๊ธฐ ์ํด labeled data์ ๊ฐ์ด ๋ชจ๋ธ์ ์ฒ์๋ถํฐ ๋ค์ ํ์ตํด์ผ ํ๋ค.

&nbsp; ๋ฐ๋ผ์ Transductive Learning ๊ฐ์ ๊ฒฝ์ฐ ์๋ก์ด unlabeled ๋ฐ์ดํฐ๊ฐ ์์ฃผ ๊ด์ธก๋๋ ์ผ์ด์ค์์ cost๊ฐ ๋น์ ์ ์๋ค. ๋ฐ๋ฉด, Inductive Learning ๊ฐ์ ๊ฒฝ์ฐ predictive model์ ์ด๊ธฐ์ ์์ฑํด๋๊ธฐ ๋๋ฌธ์ ๋ ์ ์ cost๋ก ๋น ๋ฅธ ์๊ฐ์์ ์๋ก ๊ด์ธก๋ ๋ฐ์ดํฐ์ label์ ์์ธกํ  ์ ์๋ค. ์ฐธ๊ณ ๋ก, ์ฌ๊ธฐ์ cost๋ ์ปดํจํ ํ์, ์๊ฐ, ์ฐ์ฐ๋ ๋ฑ์ ์๋ฏธํจ
<br><br>

<center>

|<h4> **TABLE 1. &nbsp Inductive Learning vs Transductive Learning** </h4>|
| :---: |
|![Inductive Learning vs Transductive Learning](https://velog.velcdn.com/images/kimdyun/post/ea851cdd-9319-4862-a47e-99419b6effe2/image.png "Inductive Learning vs Transductive Learning")|

</center>

์ ๊ทธ๋ฆผ์ด Inductive Learning๊ณผ Tranductive Learning์ ์ฐจ์ด๋ฅผ ์ ์ ๋ฆฌํ์ฌ ๋ณด์ฌ์ฃผ๋ ๊ฒ ๊ฐ์ ์ฐธ์กฐํ์๋ค.

<br><br>

### ๐ ๋์ ์์
#### &nbsp; ์ ์ฐธ์๋ค.. ์์ผ๋ก๋ ๊ทธ๋ฆผ ์์๋ฅผ ๋ณด๋ฉด์ ์กฐ๊ธ์ด๋๋ง ๋ฆด๋ ์คํ์๊ธธ ๐ค

<br>

<center>

|<h4>_Figure 1_</h4>|
|:---:|
|<img src = "https://velog.velcdn.com/images/kimdyun/post/d886ef14-f5c1-4274-a871-9aeb477e2474/image.PNG" alt = "Figure 1" width = "500">| 

</center>

<br>

&nbsp; ์ฐ์  ์ ๊ทธ๋ฆผ ์์์์ **labeled data (training data)**๋ <span style="color:red;"> **A** </span>, <span style="color:red;"> **B** </span>, <span style="color:blue;"> **C** </span>, <span style="color:blue;"> **D** </span>์ด๊ณ  <span style="color:red;"> **A** </span>์ <span style="color:red;"> **B** </span>๋ **class** <span style="color:red;"> **red** </span>, <span style="color:blue;"> **C** </span>์ <span style="color:blue;"> **D** </span>๋ **class** <span style="color:blue;"> **blue** </span>, ๋๋จธ์ง **์ซ์**๋ค์ **unlabeled data (testing data)** ์ด๋ค. ์ฌ๊ธฐ์ unlabeled data์ label์ ์ถ๋ก ํด์ผ ํ๋ ์ํฉ์ผ ๋, Inductive Learning์์๋ 4๊ฐ์ training data๋ง์ ์ฌ์ฉํ์ฌ ์ง๋ ํ์ต (supervised learning)์ ์ํํ ํ ํ์ต๋ ์์ธก ๋ชจ๋ธ์ testing data์ ์ ์ฉํ์ฌ label์ ์ถ๋ก ํ๋ฉด ๋๋ค.

<br><br>

<center>

|<h4>_Figure 2_</h4>|
|:---:|
|<img src = "https://velog.velcdn.com/images/kimdyun/post/140934d0-0fdf-411e-8512-29be3533e5a0/image.PNG" alt = "Figure 2" width = "500">|

</center>

&nbsp; ๊ทธ๋ฌ๋ Inductive Learning ๊ฒฝ์ฐ์์๋ ํ๋ จ ๋ฐ์ดํฐ๊ฐ ํฑ ์์ด ๋ถ์กฑํ๊ธฐ ๋๋ฌธ์ ์ ๋ฐ์ ์ผ๋ก label์ ์์ธกํ๋ ๋ชจ๋ธ์ ๋ง๋ค๊ธฐ ์ด๋ ค์ธ ์ ์๋ค. ์๋ฅผ ๋ค์ด, K neareast neighbor ๋ฐฉ์์ ์ ์ฉํ ๊ฒฝ์ฐ, ์ซ์ 10๊ณผ 12๋ C์ D๋ณด๋ค B์ ๋ ๊ฐ๊น๊ธฐ ๋๋ฌธ์ class red๋ก ๋ถ๋ฅ๋  ๊ฒ์ด๋ค.
> ์ฌ๊ธฐ์, ์ซ์ 10๊ณผ 12๊ฐ ์๋ชป ๋ถ๋ฅ๋์๋ค๊ณ  ๋งํ  ์๋ ์๋ค. ํ์ง๋ง, ํ์ต ๋ฐ์ดํฐ๊ฐ ์๋นํ ์ ๊ธฐ ๋๋ฌธ์ 10๊ณผ 12๊ฐ class red๋ก ๋ถ๋ฅ๋ ๊ฒ์ ๋ํด ์ฐ๋ฆฌ๋ ๋น์ฐํ๊ฒ๋ ์ ๋ขฐํ  ์ ์๋ค.

<br><br>

<center>

|<h4>_Figure 3_</h4>|
|:---:|
|<img src = "https://velog.velcdn.com/images/kimdyun/post/acc4466c-3fe5-46bf-9bc4-d8aa32f21ecc/image.PNG" alt = "Figure 3" width = "500">|

</center>

&nbsp; ๋ง์ฝ ์์ ๊ทธ๋ฆผ 3์ฒ๋ผ Non-Euclidean ๊ณต๊ฐ์์ ๊ทธ๋ํ ๋ฐ์ดํฐ์์ ๋ฐ์ดํฐ ๋ธ๋ ๊ฐ ์ฃ์ง ์ ๋ณด๊ฐ ์ถ๊ฐ๋์๋ค๊ณ  ๊ฐ์ ํ๋ค. ๋ํ, ์ด ์ฃ์ง๋ ๊ฐ์ค์น๊ฐ ์์ผ๋ฉฐ B์ 10 ๊ฐ์ ์ฃ์ง ๊ฐ์ค์น๋ ๋งค์ฐ ์๊ณ  ๋๋จธ์ง ์ฃ์ง ๊ฐ์ค์น๋ ํฌ๋ค๊ณ  ๊ฐ์ ํด๋ณธ๋ค. ์ด ๋, ์ด ์ฃ์ง์ ์ฃ์ง ๊ฐ์ค์น๋ ์ถ๊ฐ์ ์ธ ์ฐ๊ฒฐ์ฑ ์ ๋ณด๋ฅผ ์ ๊ณตํด์ค๋ค. ์์ผ๋ก ์ด ์ถ๊ฐ ์ ๋ณด๋ฅผ ์ ๊ทน ํ์ฉํด๋ณผ ๊ฒ์ด๋ค.

<br><br>

<center>

|<h4>_Figure 3_</h4>|
|:---:|
|<img src = "https://velog.velcdn.com/images/kimdyun/post/cf774459-dd10-403f-87b0-0973e18e6f92/image.PNG" alt = "Figure 4" width = "500">|

</center>

&nbsp; Inductive Learning์์๋ ์ด๋ฌํ ์ฃ์ง ์ถ๊ฐ ์ ๋ณด๊ฐ ์๋ค๊ณ  ํ๋๋ผ๋, ํ์ฉํ๊ธฐ ์ด๋ ต๋ค. ์๋ํ๋ฉด ์์์ ์ธ๊ธํ๋ฏ์ด, <span style="color:red;"> **์ฐ๋ฆฌ๋ ํ์ต ์ ์ค์ง Training dataset์ ์ ๋ณด๋ง ์ ๋ฟ, Testing dataset์ ๊ด์ธกํ ์  ์๊ธฐ ๋๋ฌธ์ด๋ค.** </span> ๋ฐ๋๋ก, **Transductive Learning**์์๋ ์ฐ๋ฆฌ๊ฐ ์ด๋ฏธ Training dataset ๋ฟ๋ง ์๋๋ผ Testing dataset๋ ์๊ณ  ์๋ค. ๋ค๋ง, Testing dataset์ label๋ง ๋ชจ๋ฅผ ๋ฟ, Testing dataset์ ๋ฐ์ดํฐ ์ ๋ณด๋ ์ถฉ๋ถํ ํ์ต ๋ ํ์ฉํ  ์ ์๋ค. ์ฌ๊ธฐ์, ์ฃ์ง ์ถ๊ฐ ์ ๋ณด๊น์ง ์ฐ๋ฆฌ๊ฐ ์๊ณ  ์๊ธฐ ๋๋ฌธ์ **์ฐ๊ฒฐ์ฑ์ ๊ธฐ๋ฐํ์ฌ Training dataset์ label์ Testing dataset์ ์ ํํ  ์ ์๋ค.** **(Graph-based label propagation algorithm, LPA)** ์ด ์์์์์ ์ ๊ทผ๋ฒ์ ์ค์ง๋ํ์ต (Semi-supervised Learning) ๋ฐฉ์์ด๋ผ๊ณ ๋ ๋ณผ ์ ์๋ค. ๊ทธ๋ฆผ 3๊ณผ ๋ค๋ฅด๊ฒ ์ด ๋๋ 10๊ณผ 12 ๋ธ๋๋ class blue๋ก ๋ถ๋ฅ๋๋ค.

### &nbsp; ๐ ํต์ฌ ํฌ์ธํธ
> Transductive Learning์์๋ ์ฐ๋ฆฌ๊ฐ ์ฌ์ ์ Testing dataset๋ ์๊ณ  ์๋ค๋ ์ ๊ณผ, ์ฃ์ง ์ ๋ณด์ ๊ฐ์ ์ ์ฉํ ์ถ๊ฐ ์ ๋ณด๋ฅผ ํ์ฉํ  ์ ์๋ค๋ ์ ์ด ํต์ฌ์ด๋ค. ๋ง์ฝ, ์ฌ์ ์ ์๊ณ ์๋ Testing dataset์ด ์๋ค๋ฉด Inductive Learning ๋ง ์ ํํ  ์ ์๋ค. **(Inductive Learning์์๋ predictive model์ ์์ฑํ๋ฏ๋ก ์๋ก์ด ๋ฐ์ดํฐ๊ฐ ์ธ์  ๊ด์ธก๋์ด๋ ์๊ด์๊ธฐ ๋๋ฌธ)**

<br><br>

### ๐ ๋ง๋ฌด๋ฆฌ
๊ฐ๋จํ ์์๋ค๊ณผ ํจ๊ป Transductive Learning๊ณผ Inductive Learning์ ์ฐจ์ด์ ๊ฐ ๋ฐฉ์์ ๊ฐ๋์ ๋ํด ์์๋ณด์๋ค. ํ์ฌ ์์ฑ์ ๋ณธ์ธ์ Graph Neural Network๋ฅผ ํ์ฉํ์ฌ Brain network์ ๊ด๋ จ๋ ์ฐ๊ตฌ๋ฅผ ์ํํ๊ณ  ์๊ธฐ ๋๋ฌธ์, ๊ทธ๋ํ ๊ธฐ๋ฐ ์์๋ฅผ ๋ค์ด ์ค๋ชํ์๋ค.

์์์ ๋ณ๊ฐ๋ก ๋ ๋ฐฉ์์ ๊ฐ๋์ ๋ณํ์ง ์์ผ๋ ์ด ๊ธ์ ์ฝ๊ณ  ๋์์ด ๋์๊ธธ ๋น๋๋ค!

<br><br>

### ๐ References
[1]  Transduction (machine learning) Wikipedia โ https://en.wikipedia.org/wiki/Transduction_(machine_learning)
[2]  Inductive vs. Transductive Learning โ https://towardsdatascience.com/inductive-vs-transductive-learning-e608e786f7d
[3]  V. Vapnik, "Transductive Inference and Semi-Supervised Learning" โ https://pdfs.semanticscholar.org/5a8c/38e6aadc29fb995d5b9562df0c4365156256.pdf
