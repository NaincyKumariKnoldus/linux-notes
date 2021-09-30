## AWK Commands
---
  ### mytext.txt file:

```this is Sneha
this is Naincy
this is Navnita.
this is Shinni.
this is Nishant.
```
 
* `awk '{print}' mytext.txt`

```this is Sneha
this is Naincy
this is Navnita.
this is Shinni.
this is Nishant.
```


* `awk '/Naincy/ {print}' mytext.txt`
 
```this is Naincy```




* `awk '{print $1,$2}' mytext.txt`
```this is
this is
this is
this is
this is
```



* `awk '{print NR,$0}' mytext.txt`
```1 this is Sneha.
2 this is Naincy.
3 this is Navnita.
4 this is Shinni.
5 this is Nishant.
```


* `awk '{print $1,$NF}' mytext.txt`
```this Sneha
this Naincy
this Navnita
this Shinni
this Nishant
```



* `awk 'NR==3, NR==6{print NR,$0}' mytext.txt`
```3 this is Navnita
4 this is Navnita
5 this is Nishant
```



* `awk '{print NR "- " $1}' mytext.txt`
```1- this
2- this
3- this
4- this
5- this
```



* `awk '{print $2}' mytext.txt`
```is
is
is
is
is
```



* `awk 'END {print NR}' mytext.txt`

```5```



* `awk 'length($0) > 9' mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Shinni.
this is Nishant.
```



* `awk '{ if($3 == "Naincy") print $0}' mytext.txt`

```this is Naincy.```



## SED Commands
---
* `sed 's/this/ it /' mytext.txt`
``` it  is Sneha.
 it  is Naincy.
 it  is Navnita.
 it  is Shinni.
 it  is Nishant.
```



* `sed 's/is/ it /2' mytext.txt`
```this  is  Sneha
this  is Naincy.
this  it  Navnita.
this  is Shinni.
this  is  Nishant.
```



* `sed 's/is/it/g' mytext.txt`
```thit it Sneha.
thit it Naincy.
thit it Navnita.
thit it Shinni.
thit it Nishant.
```



* `sed '3d' mytext.txt` 
```this is Sneha
this is Naincy.
this is Navnita.
this is Shinni.
```



* `sed '$d' mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Shinni.
```



* `sed '3,5d' mytext.txt`
```this is Sneha
this is Naincy.
```



* `sed '5,$d' mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Shinni.
```



* `sed '/is/d' mytext.txt`
```this is Naincy.
this is Navnita.
this is Shinni.
this is Nishant.
```


### GREP Commands
---
* `grep -c "this" mytext.txt`

```5 ```



* `grep -l "Sneha" *` 
```
text.txt
```



* `grep -w "Naincy" mytext.txt`

```this is Naincy.
this is Naincy.
```



* `grep -o "Sneha" mytext.txt`

```Sneha
Sneha
```



* `grep -n "Shinni" mytext.txt`
```4:this is Shinni.
this is Shinni.
```



* `grep -v "Nishant" mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Shinni.
```


* `grep "^this" mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Shinni.
this is Nishant.
```



* `grep "Naincy$" mytext.txt`

```this is Naincy.
this is Naincy.
```



* `grep -e "Naincy" -e"Navnita" -e "Nishant" mytext.txt`
```this is Sneha.
this is Naincy.
this is Navnita.
this is Nishant.
```
   
   
