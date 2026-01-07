# Week 5: JavaScript Fundamentals - Lab Summary

## แสดงผลลัพธ์ และอธิบายการทำงานของโค๊ดว่าแสดงผลลัพธ์มาได้อย่างไร

### ไฟล์ 01-variables.js

### 6. Challenge: Create a Person Object ✅

#### คำอธิบายการทำงานของโค้ด

ในไฟล์นี้เป็นการสร้าง Object ชื่อ `student` เพื่อเก็บข้อมูลของนักเรียน โดยใช้ตัวแปรแบบ Object ซึ่งสามารถเก็บข้อมูลหลายประเภทไว้ในตัวแปรเดียวได้

Object `student` ประกอบด้วย:

- `firstName` และ `lastName` (String)
- `age` (Number)
- `gpa` (Number)
- `courses` (Array)
- `isActive` (Boolean)
- `getFullName()` (Function)
- `getInfo()` (Function)

#### การทำงานทีละขั้นตอน

1. สร้าง Object `student` และกำหนดค่า property ต่าง ๆ
2. ฟังก์ชัน `getFullName()` ใช้ `this.firstName` และ `this.lastName`  
   เพื่อรวมชื่อและนามสกุลเป็นชื่อเต็ม
3. ฟังก์ชัน `getInfo()` เรียกใช้ `getFullName()`  
   และนำข้อมูลอายุ (`age`) และเกรดเฉลี่ย (`gpa`) มาแสดงผล
4. ใช้ `console.log()` แสดง:
   - Object `student`
   - ชื่อเต็ม
   - ข้อมูลนักเรียน
   - รายวิชาที่เรียน (ใช้ `join(", ")`)

#### ผลลัพธ์ที่ได้จากการรันโค้ด

```text
=== Challenge: Person Object ===
Student object:
{
  firstName: 'Alice',
  lastName: 'Smith',
  age: 20,
  gpa: 3.8,
  courses: [ 'HTML', 'CSS', 'JavaScript' ],
  isActive: true,
  getFullName: [Function: getFullName],
  getInfo: [Function: getInfo]
}
Full name: Alice Smith
Info: Alice Smith, Age: 20, GPA: 3.8
Courses: HTML, CSS, JavaScript
```
