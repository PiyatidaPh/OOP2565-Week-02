# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ไม่ได้ | null เป็นการเช็คว่าตัวแปรหรือ textbox เป็นค่าว่างหรือไม่ |
| `_value` | ใช้ได้ | _ไม่ได้เป็นตัวดำเนินการ |
| `First-name`| ไม่ได้ | - เป็นตัวดำเนินการ |
| `Hello!` | ไม่ได้ | ! เป็นตัวดำเนินการ |
| `w*h` | ไม่ได้ | * เป็นตัวดำเนินการ |
| `time` | ใช้ได้ | ไม่มีอักษรละเมิดกฎการตั้งชื่อ |
| `do` | ไม่ได้ | do เป็นคำสั่ง |
| `Do` | ใช้ได้ | Do ไม่เป็นคำสั่ง |
| `21November`| ไม่ได้ | ไม่สามารถใช้เลขเป็นชื่อตัวแปรได้ |
| `ladkrabang`| ใช้ได้ | ไม่มีอักษรละเมิดกฎการตั้งชื่อ |
| `Student ID`| ไม่ได้ | ไม่สามารถเว้นวรรคชื่อตัวแปรได้ |


---ผลการทดลอง

= ชื่อตัวแปรควรตั้งให้จำง่าย มีความหมาย ไม่สามารถใช้เครื่องหมายดำเนินการทางคณิตศาสตร์เป็นชื่อตัวแปรได้ ไม่สามารถเว้นวรรคชื่อตัวแปรได้ ไม่สามารถใช้คำที่เป็นคำสั่งมาเป็นชื่อตัวแปรได้


## ชนิดข้อมูลภายในภาษา C\#

Property ของชนิดข้อมูล ในภาษา C# มีชนิดข้อมูลต่างๆ ได้แก่ `byte`, `char`, `bool`, `sbyte`, `short`, `ushort`, `int` , `uint`, `float`, `double`, `decimal`, `long`, `ulong` โดยแต่ละชนิด มีคุณสมบัติที่สำคัญได้แก่ ขนาด (เป็นไบต์) ค่าต่ำสุด ค่าสูงสุด ที่เก็บในตัวแปรชนิดนั้นๆ ได้ ซึ่งมีฟังก์ชันในภาษา C# ที่ช่วยให้เราทราบคุณสมบัติเหล่านั้น ได้แก่คำสั่ง `sizeof()`, `MinValue()` และ `MaxValue()` การแสดงค่าคุณสมบัติต่างๆ ของตัวแปร สามารถทำได้โดยใช้ฟังก์ชั่นเหล่านั้น ดังตัวอย่าง

## 13. โปรแกรมแสดงคุณสมบัติ size, MinValue และ MaxValue ของชนิดข้อมูล

```csharp
Console.WriteLine("Data type : int");
Console.WriteLine("Size :" + sizeof(int));
Console.WriteLine("Minimum Value :" + int.MinValue);
Console.WriteLine("Maximum Value :" + int.MaxValue);
```

### ผลที่ได้จากโปรแกรม

```text
Data type : int
Size :4
Minimum Value :-2147483648
Maximum Value :2147483647
```

👉 คำสั่งสำหรับการทดลอง  

ให้นักศึกษา เขียนโปรแกรมคล้ายกับตัวอย่างในข้อ 13 โดยมีชนิดข้อมูลเป็น `byte`, `char`, `bool`, `sbyte`, `short`, `ushort`, `uint`, `float`, `double`, `decimal`, `long` `และ ulong`  

### หมายเหตุ

ชนิดข้อมูล bool เก็บข้อมูลได้เฉพาะ true และ false ไม่ต้องหา MinValue และ MaxValue

ชนิดข้อมูล char จะต้องมีการ cast ค่า MinValue และ MaxValue ไปยัง int ก่อน ดังนี้

```csharp
Console.WriteLine("Minimum Value :" + (int) char.MinValue);
Console.WriteLine("Maximum Value :" + (int) char.MaxValue);
```
---ผลการทดลอง `char`

![Screenshot 2566-01-18 at 15 16 36](https://user-images.githubusercontent.com/115066261/213118923-910cba3f-f672-4107-97e6-2bf3992a48f7.png)

---ผลการทดลอง `byte`

![Screenshot 2566-01-18 at 15 16 00](https://user-images.githubusercontent.com/115066261/213118805-7e5ab384-22cb-454b-97e4-4cc84a23dbf0.png)

---ผลการทดลอง `short`
 
![Screenshot 2566-01-18 at 15 15 24](https://user-images.githubusercontent.com/115066261/213118683-c4adf70f-cc07-4d14-bc22-8979843996e1.png)

---ผลการทดลอง `ushort`

![Screenshot 2566-01-18 at 15 14 47](https://user-images.githubusercontent.com/115066261/213118537-a419e201-da0b-456c-adbe-8a25116ef80b.png)

---ผลการทดลอง `uint`

![Screenshot 2566-01-18 at 15 14 14](https://user-images.githubusercontent.com/115066261/213118417-d831de35-5a22-4d9f-8d35-3e3ac3c979dd.png)

---ผลการทดลอง `float`
 
![Screenshot 2566-01-18 at 15 17 57](https://user-images.githubusercontent.com/115066261/213119175-74baa5c6-5d8b-4e48-9d1b-55b23fdea9d8.png)
 
---ผลการทดลอง `double`

![Screenshot 2566-01-18 at 15 18 44](https://user-images.githubusercontent.com/115066261/213119333-24be74ca-e9f3-4640-9b25-13ede8200603.png)

---ผลการทดลอง `decimal`

 ![Screenshot 2566-01-18 at 15 19 36](https://user-images.githubusercontent.com/115066261/213119469-bf35648c-3581-4497-9560-f78406b68187.png)

---ผลการทดลอง `long`

![Screenshot 2566-01-18 at 15 20 13](https://user-images.githubusercontent.com/115066261/213119620-08efdd92-0900-46d5-9819-e2db8f673358.png)

---ผลการทดลอง `ulong`

![Screenshot 2566-01-18 at 15 20 47](https://user-images.githubusercontent.com/115066261/213119724-201dae67-100e-4f4c-be3f-54a17b09d427.png)

---ผลการทดลอง `bool`

![Screenshot 2566-01-18 at 15 23 15](https://user-images.githubusercontent.com/115066261/213120221-11b6dba9-9e1d-4039-99a4-edbb5ceb2e08.png)

---ผลการทดลอง `sbyte`

![Screenshot 2566-01-18 at 15 23 51](https://user-images.githubusercontent.com/115066261/213120329-d779d4b2-a468-4d08-8363-a2057a0a09f8.png)

## การใช้งานข้อมูลชนิดต่างๆ

ข้อมูลชนิดตรรกะ The Boolean Type
ข้อมูลชนิดตรรกะ (boolean) มีค่าที่เป็นไปได้เพียง 2 ค่าเท่านั้นคือ true และ false ในภาษา C# จะไม่สามารถกำหนดค่าตัวเลขลงไปในตัวแปร boolean ได้ ส่วนใหญ่ตัวแปร boolean มักใช้เพื่อการตัดสินใจและมีที่มาจากการประเมินค่าสมการต่างๆ ตัวอย่างต่อไปนี้เป็นการใช้ตัวแปร boolean กับการเปรียบเทียบด้วยตัวดำเนินการ “>”
ตัวอย่าง

```csharp
bool a = 4 > 5;
Console.WriteLine("4 > 5 is {0}", a);
```

## สนุกกับการสร้างตัวเลขสุ่ม

ในภาษา C# มีวิธีการสร้างตัวเลขสุ่ม (random number) โดยใช้คลาส Random มาสร้างเป็นตัวแปรโดยมีรูปแบบดังนี้

```csharp
Random random = new Random();
```

เมื่อสร้างแล้ว เราสามารถนำมาหาค่าตัวเลขสุ่มจากตัวแปรดังกล่าว ซึ่งมักจะกำหนดค่าสูงสุดและต่ำสุดในการสุ่มลงไปด้วย ดังนี้

```csharp
int randomNumber = random.Next(0, 100);
```

โปรแกรมด้านล่างนี้เป็นตัวอย่างการสุ่มเลข 0 – 100

```csharp
Random random = new Random();
int randomNumber = random.Next(0, 100);
Console.WriteLine(randomNumber);
```
 
ให้รัน 10 ครั้งแล้วบันทึกค่าที่ได้จากการรัน

![Screenshot 2566-01-18 at 15 27 57](https://user-images.githubusercontent.com/115066261/213121137-4c7572a3-50c4-4cbc-bb5a-d90e9069ddb4.png)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
