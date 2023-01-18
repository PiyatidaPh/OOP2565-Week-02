# Lab-01  ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)

ข้อมูลชนิดตัวเลขจำนวนเต็ม สามารถนำไปใช้งานได้หลากหลาย เช่น การนับหรือแสดงจำนวน การกำหนดลำดับที่ การจัดลำดับ เป็นต้น ค่าที่ใส่ลงในตัวแปร เป็นได้ทั้งค่าบวก ค่าศูนย์ และค่าลบ (มีตัวแปรบางชนิดที่เก็บเฉพาะค่าบวกเพียงอย่างเดียว) การกำหนดค่าใดๆ ให้กับตัวแปร ทำได้โดยการใช้เครื่องหมาย =
การใช้เครื่องหมายคณิตศาสตร์กับตัวแปรจำนวนเต็ม สามารถใช้ได้ทุกเครื่องหมาย ได้แก่ +, -, *, / และ %

## 15. การใช้เครื่องหมายทางคณิตศาสตร์กับตัวแปรชนิดจำนวนเต็ม

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
int a, b, c, d, e, f;
a = 1;
b = a + 6;
c = b - 3;
d = c * 2;
e = d / 2;
f = e % 2;
Console.WriteLine("a={0}", a);
Console.WriteLine("b={0}", b);
Console.WriteLine("c={0}", c);
Console.WriteLine("d={0}", d);
Console.WriteLine("e={0}", e);
Console.WriteLine("f={0}", f);
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 16 03 33](https://user-images.githubusercontent.com/115066261/213128704-33c7b144-d47c-4bb0-a237-7b8189b1df4b.png)



## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`

![Screenshot 2566-01-18 at 16 06 44](https://user-images.githubusercontent.com/115066261/213129358-78778d75-8d61-47c5-89e4-e37ed3b78c67.png)

2. `x-b`

![Screenshot 2566-01-18 at 16 07 48](https://user-images.githubusercontent.com/115066261/213129591-51dff1fb-cfb4-457c-bd2a-b8606db37d6a.png)

3. `x*b`

![Screenshot 2566-01-18 at 16 08 45](https://user-images.githubusercontent.com/115066261/213129758-3c0c7356-5a6d-4344-ad73-ecacddaa1e09.png)

4. `y/a`

![Screenshot 2566-01-18 at 16 09 26](https://user-images.githubusercontent.com/115066261/213129922-5c27ab83-00a4-49df-a0bc-7a68cc4cf246.png)

5. `b%y`

![Screenshot 2566-01-18 at 16 10 21](https://user-images.githubusercontent.com/115066261/213130145-1880895b-1cc3-4b55-9833-8ca28a1930be.png)

6. `y+10%x`

![Screenshot 2566-01-18 at 16 13 33](https://user-images.githubusercontent.com/115066261/213130877-0828eefa-3dc3-400b-8d4b-5d8a2f250194.png)

7. `a/3*5`

![Screenshot 2566-01-18 at 16 14 42](https://user-images.githubusercontent.com/115066261/213131143-e6d9b3e8-8447-451e-8f97-57121ec50ed3.png)

8. `9/2*a`

![Screenshot 2566-01-18 at 16 19 52](https://user-images.githubusercontent.com/115066261/213132284-2d383300-cd67-4191-a869-c376ffef55a5.png)

9. `y%8`

![Screenshot 2566-01-18 at 16 21 38](https://user-images.githubusercontent.com/115066261/213132642-ce836c20-2ada-4cf0-b993-40ee5ababb67.png)

10. `100*x+y%2-a`

![Screenshot 2566-01-18 at 16 25 17](https://user-images.githubusercontent.com/115066261/213133492-e7a3a718-0907-4d2c-984e-a3a49c949407.png)


## ชนิดข้อมูลเลขทศนิยม (Floating Point and Decimal Types)

ตัวเลขจำนวนทศนิยม มักจะใช้ในการคำนวณทางวิทยาศาสตร์ เนื่องจากค่าในวิทยาศาสตร์ต้องการความละเอียดสูง หรือมีค่าสูงมากกว่าที่เลขจำนวนเต็มจะเก็บได้

### ตัวอย่างการแก้ปัญหาทางวิทยาศาสตร์

ระยะทางจากดาวอาทิตย์ถึงโลกคือ 93,000,000 ไมล์ เรียกว่า 1 A.U. (Astronomical Unit)
ความเร็วในการเดินทางของแสงคือ 186,000 ไมล์ต่อวินาที
ระยะทาง 1 ไมล์ คิดเป็น 1.609344 กิโลเมตร
ให้เขียนโปรแกรมหาระยะทางในการเดินทางของแสง ในหน่วยกิโลเมตรต่อวินาทีและเวลาในการเดินทางของแสงจากดวงอาทิตย์มายังโลก

## 17.  โปรแกรมคำนวณระยะทางและเวลาของแสงจากดวงอาทิตย์ถึงโลก

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
const double lightSpeed = 186000d;   // miles per second
Console.WriteLine("Light speed = {0} Mile Per second", lightSpeed);
const double mileTokm = 1.609344;
Console.WriteLine("Light speed = {0} km Per second", lightSpeed*mileTokm);
const double SunToEarthDistance =  93000000d ;  // miles
Console.WriteLine("SunToEarthDistance = {0} km", SunToEarthDistance * mileTokm);
double SunToEarthTimeOfLight = SunToEarthDistance / lightSpeed;  // miles
Console.WriteLine("SunToEarthTimeOfLight = {0} seconds", SunToEarthTimeOfLight);
Console.WriteLine("SunToEarthTimeOfLight = {0} minutes", SunToEarthTimeOfLight/60d);
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 16 27 22](https://user-images.githubusercontent.com/115066261/213133938-40e9a906-75d1-4cba-a3f9-99aff427b4de.png)


👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง

![Screenshot 2566-01-18 at 16 57 18](https://user-images.githubusercontent.com/115066261/213141129-82e884e9-4d7d-453b-85e0-bb891529374d.png)

ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km | 35,983,606 mile | 5.2 minutes
| Venus | 108,200,000 km | 67,232,363 mile | 9.7 minutes
| Earth | 149,600,000 km | 92,957,130 mile | 13.4 minutes
| Mars | 227,940,000 km | 141,635,350 mile | 20.4 minutes
| Jupiter |  778,330,000 km | 483,631,840 mile | 69.7 minutes
| Uranus | 2,873,550,000 km | 1,785,541,189 mile | 257.4 minutes
| Neptune | 4,501,000,000 km | 2,796,791,736 mile | 403.3 minutes
| Pluto | 5,945,900,000 km | 3,694,610,971 mile | 532.7 minutes



 คลาส Math ในภาษา C# มีคลาสที่เป็นตัวช่วยคำนวณทางคณิตศาสตร์ ที่ช่วยให้เราสามารถคำนวณฟังก์ชันพื้นฐานได้ อย่างรวดเร็ว ไม่ต้องพัฒนาโปรแกรมเพิ่มเติมด้วยเอง นั่นคือคลาส Math ฟังก์ชันทางคณิตศาสตร์ที่ใช้บ่อยๆ สามารถดูรายละเอียดทั้งหมดได้จาก `system.math`

 
## 20.  โปรแกรมพล็อตรูป sine wave บนหน้าจอ

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
for (float i = 0; i < Math.PI * 2.0F; i += 0.3F)
{
    Console.WriteLine("The sine of {0,10:F} = {1,-10:F6}" + spaces(Math.Sin(i)) + "*", i, Math.Sin(i));
}
string spaces(double val)
{
    string SpaceString = new String(' ', ((int)(val * 10.0)) + 10);
    return SpaceString;
}
```

หมายเหตุ ในการเขียนโปรแกรมภาษา C# .NET6.0 ที่ใช้ template แบบใหม่ เราก็ยังคงสามารถสร้าง function ใช้งานได้ตามปกติ (แต่จะไม่ครอบคลุม feature ทั้งหมดใน OOP )

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 17 58 13](https://user-images.githubusercontent.com/115066261/213154283-18863396-f530-4f18-bffa-9fa8f3c33fb9.png)
  
