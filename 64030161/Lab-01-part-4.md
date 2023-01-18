# Lab-01 Part 4 จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()

โดยทั่วไป การพิมพ์ข้อความออกทาง console สามารถพิมพ์ข้อความได้ทั้งแบบตายตัวและเปลี่ยนแปลงได้โดยโปรแกรม หากเราต้องการพิมพ์แบบตายตัวก็อาจใช้คำสั่ง `Console.WriteLine` เขียนเรียงกันไปเรื่อยๆ 

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("This is text 1.");
Console.WriteLine("This is text 2.");
Console.WriteLine("This is text 3.");
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 32 32](https://user-images.githubusercontent.com/115066261/213084637-f49ff902-d7c1-41d8-8659-3d4e65289847.png)

ถ้าหากต้องการให้แก้ไขค่าตัวแปรที่จะแสดงออกทาง console เราก็อาจจะใช้ป้ายกำกับสำหรับรับค่าออกไปแสดงที่ output เรียกว่า place holder

การนับลำดับ place holder จะเริ่มจากตัวแรกที่มีค่าเป็น 0

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine(" {0} and {1}", 3, 6);
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 34 09](https://user-images.githubusercontent.com/115066261/213084828-86ae5907-2e3b-49ad-bbd0-c738a20b4188.png)

❔ ถ้ามีการใช้ตัวเลขใน { } ที่กระโดด เช่น {0} {2} {3} จะใช้งานได้หรือไม่ อย่างไร จงอธิบาย

= ใช้งานไม่ได้ เพราะ ป้อนค่า Input ไม่ถูกต้อง

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("{1}, {0} and {1}", 3, 6);
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 37 59](https://user-images.githubusercontent.com/115066261/213085288-6bd678d0-12fe-4f33-b33b-11b02e2f6415.png)

 
## [5. การกำหนดความกว้างของอาร์กิวเมนต์](./Lab-01-part-5-7.md)
