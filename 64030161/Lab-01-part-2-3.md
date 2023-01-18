# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 07 52](https://user-images.githubusercontent.com/115066261/213081447-1f5d7857-4ef0-4ebf-84f6-0eae66d44640.png)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

= คำว่า Hello แสดงบนหน้่าจอในบรรทันเดียวกันและติดกัน 

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 12 27](https://user-images.githubusercontent.com/115066261/213081929-172cc6c7-aca6-4586-9002-b4e52747e575.png)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

= คำว่า Hello แสดงบนหน้าจอ 2 บรรทัด โดยหลังจากแสดงคำว่า Hello คำแรกแล้วก็ขึ้นบรรทัดใหม่และแสดงคำว่า Hello อีกครั้งและขึ้นบรรทัดใหม่

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 17 45](https://user-images.githubusercontent.com/115066261/213082801-cd721c8e-4f2c-4f8c-a5fd-03cc806978dd.png)

แสดงคำว่า Hello และขึ้นบรรทัดใหม่

👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2566-01-18 at 11 20 08](https://user-images.githubusercontent.com/115066261/213083117-3a8e8047-5fa3-4996-80c9-4fb2bf3bd76f.png)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

= เป็นอย่างที่คิด Console.Write เป็นคำสั่งให้แสดงผลข้อความ Hello และยังไม่ได้สั่งให้ขึ้นบรรทัดใหม่ คำสั่งConsole.WriteLine สั่งให้แสดงผลคำว่า World และค่อยขึ้นบรรทัดใหม่ทำให้คำว่า
  Hello Wrold อยู่ในบรรทัดเดียวกัน

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
= Console.Write จะแสดงผลข้อความตามที่กำหนดโดยจะไม่ขึ้นบรรทัดใหม่จนกว่าจะมีคำสั่ง เช่น \n หรือ Environment.NewLine
  Console.WriteLine จะแสดงผลข้อความตามที่กำหนดจากนั้นจะขึ้นบรรทัดใหม่

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
