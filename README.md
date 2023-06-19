با تشکر از تمام دوستانی که زحمت کشیدند برای اینترنت آزاد.

ممنون از سگارو، وحید و IRCF

چون برای خودم خیلی سخت بود تک تک دامنه ها رو چک کنم و لیست طولانی هم داره

این کد مبتدی کوچیک رو نوشتم اینکه پیدا کردن SNI راحت تر باشه متناسب با اینترنت شما، به جای اینکه تک تک دستی چک کنیم.

من کاملا مبتدی هستنم، و قطعا این کد حرفه ای نیست و یکم کار راه انداز هستش. شرمنده

کافیه از داخل سایت bgp.tools، لیست مورد نظرتون رو به صورت یک جا کپی کنید، به عنوان مثال

	A	DNS
	37.59.0.8	www.dylemo.pl, dylemo.pl
	37.59.0.18	www.kisland.com, kisland.com
	37.59.0.116	stage.mozilla-hispano.org, foroestatico.mozilla-hispano.org ( 5 more...)
	37.59.0.183	shinken.2le.net
 	.
	.
 	.
  	.


وقتی که کلا دیتا رو کپی کردید، داخل یک فایل txt سیو کنید.

نمونه ای که من کپی کردم

![Domains](https://github.com/NoAnyNameForMe/SNI-Checker/assets/137012307/65fd6fcf-5ad2-4968-be78-26a7e277a8d2)


بعد کد رو ران کنید، از شما مسیر فایل txt میپرسه که کامل وارد کنید. به عنوان مثال

	C:/SNI/domains.txt

بعد خود کد میاد دامنه ها رو جدا میکنه و اضافه هایی که مربوط به دامنه نمیشه رو حذف میکنه و شروع میکنه به پینگ گرفتن از دامنه ها.

در نهایت دامنه هایی که پینگ داشتید رو به صورت یه تیبل با پینگ به شما نشون میده.

نتیجه کار به این صورت خواهد بود که دو تا تیبل به شما نشون میده.

اول نتیجه همه رو نشون میده.

![All](https://github.com/NoAnyNameForMe/SNI-Checker/assets/137012307/38273896-1187-422b-8f58-6d1a41472a47)

و تیبل دومی هم فقط اونایی که بهشون پینگ داشتید.

![Final](https://github.com/NoAnyNameForMe/SNI-Checker/assets/137012307/8ebe2aaf-a16f-41fc-bbab-d619e05e5996)
