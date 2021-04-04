# Buuoj记录
## 1.凯撒？替换？呵呵!
MTHJ{CUBCGXGUGXWREXIPOYAOEYFIGXWRXCHTKHFCOHCFDUCGTXZOHIXOEOWMEHZO}<br>
注意：得到的 flag 请包上 flag{} 提交, flag{小写字母}

用[工具](https://quipqiup.com/)直接爆破

![](https://github.com/Cchieko/Nep/blob/main/images/cs4.png)

得到FLAG{ SUBSTITUTION CIPHER DECRYPTION IS ALWAYS EASY JUST LIKE A PIECE OF CAKE}<br>
注意提交格式，需转换为小写字母并删除空格。
flag{substitutioncipherdecryptionisalwayseasyjustlikeapieceofcake}

## 2..权限获得第一步
你猜这是什么东西，记得破解后把其中的密码给我。答案为非常规形式。 
<br>注意：得到的 flag 请包上 flag{} 提交

![](https://github.com/Cchieko/Nep/blob/main/images/2.1.png)

用MD5解密F4AD50F57683D4260DFD48AA351A17A8

得到flag为flag{3617656}

![](https://github.com/Cchieko/Nep/blob/main/images/2.2.png)

## 3.robomunication
打开音频文件，只有bi和bu的音，猜测用到摩斯密码。<br>
整理得到：… . .-… .-… — .-- … .- - … … - … . -.- . -.-- … - … … -… — --- .–. -… . . .–.

解码得到：HELLOWHATISTHEKEYITISBOOPBEEP
flag{BOOPBEEP}

##  4.Windows系统密码

![](https://github.com/Cchieko/Nep/blob/main/images/3.1.png)

MD5一个个解密，对ctf:1002:06af9108f2e1fecf144e2e8adef09efd:a7fcb22a88038f35a8f39d503e7f0062:::中的第二条32位字符数据进行MD5解密，得到flag{good-luck}.

## 5.[BJDCTF 2nd]cat_flag
gif中两种小猫分别对应二进制数0和1，则下图可用二进制表示为
01000010010010100100010001111011010011010010000101100001001100000111111001111101
再将其转换为字符串得到BJD{M!a0~}.

![](https://github.com/Cchieko/Nep/blob/main/images/4.1.png)


## 6.[BJDCTF 2nd]燕言燕语-y1ng
题目：小燕子，穿花衣，年年春天来这里，我问燕子你为啥来，燕子说:
79616E7A69205A4A517B78696C7A765F6971737375686F635F73757A6A677D2

考虑是个十六进制序列，将其转化为字符串得yanzi ZJQ{xilzv_iqssuhoc_suzjg}.

猜测使用了维吉尼亚密码，将yanzi作为密钥进行解密得到BJD{yanzi_jiushige_shabi}

## 7.传统知识+古典密码

根据六十甲子相关数表得到各个年份对应的数字，根据提示，一甲子为60年，每个数字再加上60，得到八个数字88 90 83 68 77 70 76 90，猜测为ASCII码，解码得到XZSDMFLZ

![](https://github.com/Cchieko/Nep/blob/main/images/7.1.png)

古典密码就用栅栏和凯撒密码一次尝试，最后找到SHUANGYU

![](https://github.com/Cchieko/Nep/blob/main/images/7.2.png)

## 8.[GKCTF2020]小学生的密码学

e(x)=11x+6(mod26)

密文：welcylk

（flag为base64形式）

观察是仿射加密，解密得到sorcery

![](https://github.com/Cchieko/Nep/blob/main/images/8.1.png)

flag为base64形式，转换一下得到flag{c29yY2VyeQ==}

## 9.信息化时代的步伐
也许中国可以早早进入信息化时代，但是被清政府拒绝了。附件中是数十年后一位伟人说的话的密文。请翻译出明文(答案为一串中文！)
注意：得到的 flag 请包上 flag{} 提交
密文：606046152623600817831216121621196386

标准中文电码：中国汉字多达6万字，常用的汉字只有一万个左右， 所以用10的4次方（10,000）来表示。中文电码表采用了四位阿拉伯数字作代号，简称“四码电报”，从0001到9999按四位数顺序排列，用四位数字表示最多一万个汉字、字母和符号。汉字先按部首，后按笔划排列。字母和符号放到电码表的最尾。

用[中文电码工具](http://code.mcdvisa.com/)查询对应中文得到：计算机要从娃娃抓起

## 10.[BJDCTF 2nd]灵能精通-y1ng
身经百战的Y1ng已经达到崇高的武术境界，以自律克己来取代狂热者的战斗狂怒与传统的战斗形式。Y1ng所受的训练也进一步将他们的灵能强化到足以瓦解周遭的物质世界。借由集中这股力量，Y1ng能释放灵能能量风暴来摧毁敌人的心智、肉体与器械。

给文件添加后缀.jpg,得到图片：

![](https://github.com/Cchieko/Nep/blob/main/images/10.1.png)


用到的是猪圈密码的变形，圣堂武士密码，解密得到flag{IMKNIGHTSTEMPLAR}。

猪圈密码，一种以格子为基础的简单替代式密码：

![](https://github.com/Cchieko/Nep/blob/main/images/10.2.png)


圣堂武士密码(Templar Cipher)，共济会的“猪圈密码”的一个变种：

![](https://github.com/Cchieko/Nep/blob/main/images/10.3.png)
