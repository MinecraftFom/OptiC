# OptiC
**我优化了（某种意义上）c语言的代码，让他像汇编（就是汇编的风格，不是语法），减少了输入符号的过程，只需要空格和字母就能搞定。**
                                      
**I optimized (not really) c's code to let it looks more like assembly's style. While coding, you don't need to type in symbols, only using spaces and charactors are needed.**


*如何使用 How To Use
..........................................................................................................................................................................*

crt is     struct

dl  is     while(1)

let is     auto

gt  is     typeof

td  is     typedef

use is     struct


equ   is   ==

isnt  is   !=

NULL  is   0x00

syns  is   :

ed    is   ;

val   is   =


pint  is   int*

strg  is   const char*


bs    is   [

be    is   ]

bss   is   (

bse   is   )

s     is   {

e     is   }

c     is   ,

cp    is   .

pcp   is   ->

and   is   &&

or    is   ||

sw    is   switch

ca    is   case

df    is   default   :

p     is   *

gl    is   &


by    is   *

dv    is   /

mn    is   -

pl    is   +

of    is   :

in    is   ::

git   is   %%


addr  is   ++

minr  is   --


ae    is   +=

me    is   -=

bye   is   *=

de    is   /=


ext   is   extern

em    is   enum

un    is   union

co    is   const

ch    is   char

it    is   int

db    is   double

fl    is   float

inl   is   inline

lg    is   long

res   is   restrict

sh    is   short

sd    is   signed

sta   is   static

v     is   void

vt    is   volatile

vret  is   return ed

ret   is   return

t     is   if

el    is   else

eif   is   else if

ap(any, any, any) : 
build: #define ap(init_var, append_name, value /*value's value can be NULL, 0x00*/)if(value!=NULL){typeof(init_var)init_var##append_name=value}else{typeof(init_var)init_var##append_name=NULL}
usage: example...
/*C Code
 * char hello;
 * ap(hello, __hhh,"hello~")

 * //now, hello__hhh's value is hello~
 */

gbrv(any) : 
build: #define gbrv(var) return #var
usage: example...
/*C Code
 * #define a_new_func(name) printf(gbrv(name))
 */

**备注： 不要问作者为什么给变量取这个名字，反正就是我想，没有其他原因，没有其他含义**
**P.S. Don't ask the author why named the global vars like this, that's all I want, no other reasons, no other meanings.**
