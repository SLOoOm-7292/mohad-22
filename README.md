# mohad-22
وصف المشروع راح نسوي مشروع Arduino الي هي حصالة ذكية تقتصر على العملات الحديدية ويحدد قيمتها من خلال حساس او جهاز استشعار مع وجود شاشة تحسب مجموع العملات التي بالحصالة

غداً هو اليوم الحاسم سنأتي بالقطع اللازمه لنكمل مشروعنا المبهر. ولن يكون امامنا الا برمجة القطع وهيكل المشروع

القطع اللازمة : ١* اردوينو اونو ٣* مستشعر تجنب الحواجز بالاشعة تحت الحمراء ١* سلك اردوينو ١* شاشة كريستال (LCD216) ١ لوحة تجارب حجم كبير ١* مقاومة متغيرة ١* حزمة اسلاك توصيل (ذكر - ذكر) ١* حزمة اسلاك توصيل (ذكر - انثى) 1* 40 رأس دبوس



المملكة العربية السعودية￼￼￼￼￼￼￼￼￼ المؤسسة العامة للتدريب التقني والمهني الكلية التقنية بالأحساء
التقرير الفني للتدريب التعاوني للفصل التدريبي الثاني 5441هـ
اسم المشروع : حصالة ذكية
اسم المتدرب: محمد جاسم الناصر الرقم الأكاديمي:552202244 اسم المتدرب: سلمان شاطر المطوع الرقم الأكاديمي: اسم المتدرب: محمد حسن الفرحان الرقم الأكاديمي:
التخصص: تقنية برمجة الويب وتطويره . المشرف العلمي بالكلية: أ . سامي العامر .
￼￼￼￼￼￼￼￼￼￼￼
المحتوى￼￼￼￼￼￼￼￼￼
 نبذة عن المشروع  الأكواد المستخدمة  خطوات التركيب  المصادر
￼￼￼
نبذة عن المشروع￼￼￼￼￼￼￼￼￼
عول حصالح ركيح تفيذ الفشد في هرشفيح كين هلصيىل هيي هيذنشاخ كٌيى هيي التلذي والتسليح وحافض ل .
وه فكشج هثتكشج تسيطح عذاد يقىم ترذ أي ش يرثش أهاه وسىف يتن اضافح هجسن هصٌى هي الخشة شثي تاللصيالح لكي يكيىى هتخصي في احصيا عذد القطع الورذًيح الراتشج .
￼￼￼
أكىاد الوستخذهح :￼￼￼￼￼￼￼￼￼
>include <Wire.h# >include <LiquidCrystal_I2C.h# ;)LiquidCrystal_I2C lcd(0x27, 16, 2
               ;const float coinA = A0
                 ;const int coinB = A1
                 ;const int coinC = A2
                          ;float irA=0
                      ;int irB,irC = 0
                         ;float cntA=0
         ;float cntB,cntC,cnttotal = 0
                          )(void setup
{                                     
                   ;)Serial.begin(9600
                ;)pinMode(coinA ,INPUT
                ;)pinMode(coinB ,INPUT
                 ;)pinMode(coinC,INPUT
                   ;)(lcd.begin
               ;)(lcd.backlight
}
                           )(void loop
{                                     
              ;)irA =digitalRead(coinA
              ;)irB =digitalRead(coinB
               ;)irC=digitalRead(coinC
};)if(irA ==LOW){cntA+=0.50; delay(600 };)if(irB ==LOW){cntB+=1; delay(600 };)if(irC ==LOW){cntC+=2; delay(600
             ;cnttotal =cntA+cntB+cntC
                   ;)lcd.setCursor(0,0
                  ;)":lcd.print("Total
                   ;)lcd.setCursor(8,0
                  ;)lcd.print(cnttotal
                  ;)lcd.setCursor(13,0
                     ;)"lcd.print("SAR
}                                     
￼￼￼
نطىاخ التشكية للوششو :￼￼￼￼￼￼￼￼￼ قوٌا تتىصيل 3 حساساخ sensors IR تالاسدويٌى هع الوٌافز A2 A0 A1
قوٌا تتىصيل الشاشح LCD هع الاسدويٌى ف الوٌافز A4 A5
تن التأكذ هي التىصيل تشكل صليح .
قوٌا تثشهجح الاسدويٌى تليث يقىم تأنز قشا اخ اللساساخ وهي ثن جوع قيوح الوذنلاخ الٌقذيح
قوٌا تثشهجح الشاشح لرشض قيوح الٌتائج الخاصح تاللساساخ
تن تىصيل هصذس الطاقح POWER SUPPLY تالجهاص وفصل سلك USB هي الاسدويٌى
￼￼￼￼￼
هصادس تن الشجى إليها .￼￼￼￼￼￼￼￼￼ 1- اليىيتيىب 2- هتصفح قىقل . 3- وصذيق هتخشج .
تطثيقاخ وصفلاخ الىية وتشاهج الىية الوستخذهح ؟ اليىتيىب – هكتة الكليح – هلشس اسد ويٌى – وتساب – قىقل .
￼￼￼






اعضا المجموعة : 1- محمد جاسم 2- سلمان المطوع 3- محمد الفرحان

