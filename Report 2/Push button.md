
# نام آزمایش :
خاموش و روشن کردن LED توسط push button 

## هدف :
* 1 آشنایی با push button
* 2 خاموش و روشن کردن یک LED توسط آردینو


## وسایل مورد نیاز :
* 1 بورد اردینو
* 2 یک LED
* 3 مقاومت 220 اهم و یک ۳ کیلواهم
* 4 برد بورد
* 5 کابل  USB  برای اتصال بورد اردینو به کامپیوتر
* 6 push button 


  ## شرح آزمایش :
  * 1 ابتدا LED را روی برد بورد قرار میدهیم.
  * 2 مقاومت 220 اهمی را به سر منفی (کاتد ، کوتاه تر) وصل میکنیم.
  * 3 سر دیگر مقاومت را به Gnd بورد آردینو (زمین) وصل میکنیم.
  * 4 پایه مثبت (آند ، بلندتر) LED را به پایه شماره 13 بورد آردینو وصل میکنیم.
* 5 یک push button را روی برد قرار میدهیم به طوریکه پایه ها روبروی هم باشند(عمودی)
نکته: پایه های روبرو در push button به هم متصل هستند
* 6  پایه سمت راست بالای push button را به ۵ ولت در بورد آردینو وصل میکنیم
* 7 پایه سمت چپ بالای push button را به پایه شماره ۲ وصل آردینو میکنیم
* 8 پایه سمت چپ پایین push button را به مقاومت ۳ کیلواهم وصل میکنیم 
* 9 مقاومت ۳ کیلو اهمی را به زمین وصل میکنیم 
  * 10 بورد اردینو را توسط کابل  USB  به کامپیوتر وصل میکنیم.

 
  ## کد آزمایش :
const  int but = 2 ;

const  int led = 13 ;

int buttonstate = 0 ;
  
void setup() 

{

pinMode (led , OUTPUT);

pinMode (but , INTPUT_PULLUP);

}

void loop() 

{

buttonstate = digitalRead(but);

if (buttonstate == HIGH)

{

digitalWrite (led , HIGH);

}

else

{

digitalWrite(led , LOW);

}

}

## شماتیک مدار:
![توضیح تصویر](https://github.com/Rahel12384/Microprocessor-3/blob/main/Report%202/4.jpg)


## خروجی آزمایش
![alt text](https://github.com/Rahel12384/Microprocessor-3/blob/main/Report%202/VID_20241028_070919_628.gif)


## روش صحیح گذاشتن push button 
![توضیح تصویر](https://github.com/Rahel12384/Microprocessor-3/blob/main/Report%202/IMG_20241014_103640.jpg)
 
  
## نتیجه گیری: 
در صورت فشردن دکمه ، LED روشن میشود و در صورت فشار ندادن خاموش میشود
