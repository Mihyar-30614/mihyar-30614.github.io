---
layout: post
title:  "كيفية تغيير كلمة مرور روت في SQL"
date:   2016-07-08 
categories: jekyll update
---
.ﺑﺴﻢ اﻟﻠﻪ اﻟﺮﺣﻤﻦ اﻟﺮﺣﻴﻢ

MySQL ﺳﻨﺘﺤﺪﺙ اﻟﻴﻮﻡ ﻋﻦ ﻛﻴﻔﻴﺔ ﺗﻐﻴﻴﺮ ﻛﻠﻤﺔ ﻣﺮﻭﺭ ﺭﻭﺕ ﻓﻲ

ﻓﻲ ﺣﺎﻝ ﻗﻤﺖ ﺑﺘﻌﻴﻴﻦ ﻛﻠﻤﺔ ﺳﺮ ﻋﻨﺪ ﺗﺜﺒﻴﺖ البﺮﻧﺎﻣﺞ ﻭﻗﺮﺭﺕ ﺗﻐﻴﻴﺮﻫﺎ ﻛﻞ ﻣﺎ ﻋﻠﻴﻚ ﻓﻌﻠﻪ ﻫﻮ اﺗﺒﺎﻉ اﻟﺨﻄﻮاﺕ اﻟﺘﺎﻟﻴﺔ:

1) قم بالدخول الى قاعدة البيانات من خلال الامر التالي

{% highlight ruby %}
mysql -u root -p
{%endhighlight ruby%}

2) ثم قم بتنفيذ الاوامر التالية بنفس الترتيب:

{% highlight ruby %}
use mysql;
SET PASSWORD FOR 'root'@'localhost' = PASSWORD('كلمة السر الجديدة');
{%endhighlight ruby%}

يمكنك ترك التنصيص فارغ في حال لم ترد وضع كلمة مرور.