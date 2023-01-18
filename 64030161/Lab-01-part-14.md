# Lab-01 การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวแปรชนิด boolean มักจะถูกใช้เป็นที่เก็บผลที่เกิดจากการดำเนินการทางตรรกะ เช่น AND, OR, NOT เป็นต้น ซึ่งการดำเนินการทางตรรกะจะมีตารางความจริง เป็นตัวบอกผลในการดำเนินการของตัวดำเนินการต่างๆ ดังตัวย่าง

### ตัวดำเนินการ AND

Y = A AND B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ OR

Y = A OR B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ NOT

Y = NOT A

| A | Y |
|--|--|
| 0 | 1 |
| 1 | 0 |

ตัวดำเนินการในภาษา C#
ใช้เครื่องหมายต่างๆ ดังต่อไปนี้

| การดำเนินการ | เครื่องหมาย |
|------------|-----------|
| Logical AND | & |
| Logical XOR | ^ |
| Logical OR | \| |

## 14. การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวอย่างภาษา C# ต่อไปนี้เป็นการพิมพ์ตารางความจริงออกทางหน้าจอ
👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
bool A, B,Y;
Console.WriteLine("      Y = A AND B");
Console.WriteLine("-----------------------");
Console.WriteLine("   A      B\t|  Y");
Console.WriteLine("-----------------------");
A = false; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A,B,Y);
A = false; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
Console.WriteLine("-----------------------");
```

➢ รันโปรแกรมและบันทึกผล

 ![Screenshot 2566-01-18 at 15 45 18](https://user-images.githubusercontent.com/115066261/213124890-3393059f-2cae-4704-aa5e-e68b6cf96c4c.png)

👷 จากข้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`

 ![Screenshot 2566-01-18 at 15 45 18](https://user-images.githubusercontent.com/115066261/213124890-3393059f-2cae-4704-aa5e-e68b6cf96c4c.png)

2. `OR`

![Screenshot 2566-01-18 at 15 44 27](https://user-images.githubusercontent.com/115066261/213124666-e559b5c8-faf4-4633-beee-e038c040bbb8.png)

3. `NOT`

![Screenshot 2566-01-18 at 15 50 46](https://user-images.githubusercontent.com/115066261/213125978-86d02beb-a8f6-46a7-8d3b-0adf22c87040.png)

4. `NAND`

![Screenshot 2566-01-18 at 15 57 49](https://user-images.githubusercontent.com/115066261/213127452-6a7acc00-ffa7-4d79-839d-bcf8d230e80c.png)

5. `NOR`

![Screenshot 2566-01-18 at 15 59 50](https://user-images.githubusercontent.com/115066261/213127866-bbd9fd00-277c-498e-95df-e5d4a537e563.png)

6. `Exclusive OR`

![Screenshot 2566-01-18 at 15 53 38](https://user-images.githubusercontent.com/115066261/213126561-1adf511c-c768-4e6b-86d7-4e5dd4d49f72.png)

## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
