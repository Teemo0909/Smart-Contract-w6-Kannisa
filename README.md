# Bank DApp — Assignment 6

เว็บ DApp สำหรับใช้งาน Smart Contract ระบบธนาคาร เชื่อมต่อผ่าน MetaMask และใช้งานฟังก์ชัน Deposit, Withdraw และ CheckBalance

- **รหัสนักศึกษา:** 66080904
- **ชื่อ-สกุล:** กันต์ณิษา อินตรา
- **มหาวิทยาลัย:** มหาวิทยาลัยศรีปทุม คณะเทคโนโลยีสารสนเทศ
- **เว็บ DApp (GitHub Pages):** https://teemo0909.github.io/Smart-Contract-w6-Kannisa/
- **Contract address (Sepolia):** 0x3053d5EF8D59E529F3fF8B205c2f4560aFF72144

## ไฟล์ใน repo

- `Bank.sol` — Smart Contract ระบบธนาคาร (Solidity ^0.8.0)
- `index.html` — หน้าเว็บ DApp (HTML + CSS + JavaScript ใช้ ethers.js v6)

## การทำงานของหน้าเว็บ

หน้าเว็บแสดงรหัสนักศึกษาและชื่อ-สกุล เมื่อกดปุ่ม "เชื่อมต่อ MetaMask" จะขอสิทธิ์เข้าถึงบัญชี สลับไป Sepolia ให้อัตโนมัติ และตรวจว่ามี Smart Contract อยู่ที่ address ที่กำหนดจริง จากนั้นผู้ใช้สามารถฝากเงินด้วย `deposit()` ถอนเงินด้วย `withdraw(amount)` และดูยอดเงินของบัญชีตัวเองด้วย `checkBlance()` (สะกดตามโจทย์) โดยหน้าเว็บจะแสดงสถานะและ transaction hash ของแต่ละรายการ

## การ Deploy ด้วย Remix

1. เปิด https://remix.ethereum.org สร้างไฟล์ `Bank.sol` แล้ววางโค้ด
2. Compile ด้วย Solidity 0.8.x
3. แท็บ Deploy & Run เลือก Environment เป็น Injected Provider - MetaMask (Sepolia)
4. กด Deploy แล้วนำ contract address ไปใส่ที่ `CONTRACT_ADDRESS` ใน `index.html`

## เทคโนโลยี

Solidity, Remix IDE, MetaMask, ethers.js v6, GitHub Pages
