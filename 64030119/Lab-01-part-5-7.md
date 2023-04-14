# Lab-01 Part 5 การกำหนดความกว้างของอาร์กิวเมนต์

เราสามารถแกหนดตำแหน่งของอักขระที่จะพิม์ออกทาง output ได้ โดยการใช้รูปแบบ { i, j }
โดย i ยังคงเป็นลำดับที่ตามตำแหน่งของ place holder และ j คือจำนวนช่องว่างทีต้องการ

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("00000000011111111112");
Console.WriteLine("12345678901234567890");
Console.WriteLine("{0, 0}", 1);
Console.WriteLine("{0, 1}", 1);
Console.WriteLine("{0, 2}", 1);
Console.WriteLine("{0, 3}", 1);
Console.WriteLine("{0, 5}", 1);
Console.WriteLine("{0, 10}", 1);
Console.WriteLine("{0, 15}", 1);
Console.WriteLine("{0, 20}", 1);
```

หมายเหตุ ตัวเลขสองบรรทัดบนสุด ใช้เพื่อกำหนดตำแหน่ง column ของตัวอักษร

➢ รันโปรแกรมและบันทึกผล
![image](https://user-images.githubusercontent.com/115066285/232011770-05068fd0-cf76-41a4-be1e-9cc58c37f759.png)

 
❔ การกำหนดความกว้างของอาร์กิวเมนต์ด้วยเครื่องหมาย { , } ในคำสั่ง ``Console.WriteLine()`` มีรูปแบบการใช้งานอย่างไร
ใน {} จะมีเลข 2 จำนวนแรก คือ เลขที่ต้องการให้แสดง จำนวนที่ 2 คือ ตำแหน่งตัวอักษรในบรรทัดที่ต้องการให้เลขนั้นแสดง เช่น Console.WriteLine("0,50}",1); เลข1 จะแสดงในตำแหน่งที่ 50 ของบรรทัดนั้น


## 6. การกำหนดรูปแบบของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 0:E}", n);
Console.WriteLine("{0, 0:F}", n);
Console.WriteLine("{0, 0:G}", n);
Console.WriteLine("{0, 0:N}", n);
Console.WriteLine("{0, 0:P}", n);
Console.WriteLine("{0, 0:X}", n);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://user-images.githubusercontent.com/115066285/232012855-8d0156b7-9de9-4883-8403-5a343555a828.png)

❔  การกำหนดตัวอักษร E, F, G, N, P, X หมายถึงให้พิมพ์ออกมาเป็นอะไร
  E : เป็นทศนิยม
  F : เป็นเลขจำนวนเต็มที่มีทศนิยม 2 ตำแหน่ง
  G : เป็นจำนวนเต็มที่ไม่มี ,
  N : เป็นจำนวนเต็มที่มี , และมีทศนิยม 2 ตำแหน่ง
  P : เป็นเปอร์เซ็น
  X : เป็นเลข 16 บิต

## 7. การกำหนดรูปแบบพร้อมความกว้างของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 20:E}", 1);
Console.WriteLine("{0, 20:F}", 1);
Console.WriteLine("{0, 20:G}", 1);
Console.WriteLine("{0, 20:N}", 1);
Console.WriteLine("{0, 20:P}", 1);
Console.WriteLine("{0, 20:X}", 1);
```

➢   รันโปรแกรมและบันทึกผล
![image](https://user-images.githubusercontent.com/115066285/232013976-b8d85c81-d0cd-42cd-8320-42dfad6d0372.png)
แสดงผลจากขวามาซ้ายเริ่มที่ตำแหน่งที่ 20
 
## [Part 8  การกำหนดรูปแบบพร้อมความกว้างของทศนิยมของอาร์กิวเมนต์](./Lab-01-part-8.md)