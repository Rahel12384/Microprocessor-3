# نمایش توابع سینوس و کسینوس در آردینو


## هدف :

* 1 آشنایی با برنامه نویسی
* 2 آشنایی با آردینو
* 3 نمایش توابع سینوس و کسینوس در آردینو


## وسایل مورد نیاز :

* 1 بورد اردینو
* 2 کابل  USB  برای اتصال بورد اردینو به کامپیوتر


  ## شرح آزمایش :
به پورت ۹۶۰۰ متصل می‌شویم.
از سر برگ tools وارد قسمت serial plotter  می‌شویم و روی 9600 bound  تنظیم میکنیم 

 
  ## کد آزمایش :
  
void setup() 

{

Serial.begin (9600);

}

void loop() 

{

for (float i= 0 ; i < 360.00 ; i++)

{  

 Serial.print(sin(i *(PI / 180.00)));

  Serial.print(" ");
 
   Serial.println(cos(i *(PI / 180.00)));

  }

}
  ## شرح آزمایش :
  با تابع Serial.begin به پورت 9600 متصل می شویم.از سربرگ tools قسمت serial plotter را انتخاب کرده و روی 9600baud می گذاریم و بعد موج های سینوس و کسینوس نمایش داده می شوند.
 

}

}

 ## خروجی آزمایش:
![alt text](https://github.com/Rahel12384/Microprocessor-3/blob/main/Report%201/4_5814513282077168430.gif)

 
  
## نتیجه گیری:
 این برنامه موج های سینوسی و کسینوسی را در serial plotter نشان میدهد
