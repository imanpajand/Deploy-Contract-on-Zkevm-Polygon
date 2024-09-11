 ایجاد یک اسمارت کانترکت ساده با استفاده از Remix IDE و دیپلوی آن روی شبکه zkEVM:

 ▎1. ورود به Remix

به وب‌سایت [Remix IDE](https://remix.ethereum.org/) بروید.

▎2. ایجاد یک فایل جدید

1. در پنل سمت چپ، روی آیکون "+" کلیک کنید تا یک فایل جدید ایجاد کنید.
2. نام فایل را MySimpleContract.sol بگذارید.


▎3. نوشتن اسمارت کانترکت

کد زیر را در فایل MySimpleContract.sol وارد کنید:

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract MySimpleContract {
    uint public value;

    function setValue(uint _value) public {
        value = _value;
    }

    function getValue() public view returns (uint) {
        return value;
    }
}



▎4. کامپایل کردن اسمارت کانترکت

1. به تب "Solidity Compiler" بروید (آیکون مربوط به کامپایلر).
2. نسخه Solidity را به 0.8.0 یا بالاتر تنظیم کنید.
3. روی دکمه "Compile MySimpleContract.sol" کلیک کنید.

▎5. اتصال به شبکه zkEVM

برای دیپلوی اسمارت کانترکت، شما باید به شبکه zkEVM متصل شوید. این کار را می‌توانید با استفاده از MetaMask انجام دهید:

1. نصب MetaMask: اگر هنوز این افزونه را ندارید، آن را نصب کنید.
2. تنظیم شبکه zkEVM: 
   - به MetaMask بروید و روی "Networks" کلیک کنید.
   - گزینه "Add Network" را انتخاب کنید و اطلاعات زیر را وارد کنید:
     - Network Name: zkEVM
     - New RPC URL: (آدرس RPC شبکه zkEVM)
     - Chain ID: (شماره شناسایی شبکه)
     - Currency Symbol: (نماد ارز، مانند ETH)
     - Block Explorer URL: (آدرس اکسپلورر بلاک)

▎6. دیپلوی اسمارت کانترکت

1. به تب "Deploy & Run Transactions" بروید.
2. مطمئن شوید که محیط (Environment) را روی "Injected Web3" تنظیم کرده‌اید تا به MetaMask متصل شود.
3. روی دکمه "Deploy" کلیک کنید.

▎4. کامپایل کردن اسمارت کانترکت

1. به تب "Solidity Compiler" بروید (آیکون مربوط به کامپایلر).
2. نسخه Solidity را به 0.8.0 یا بالاتر تنظیم کنید.
3. روی دکمه "Compile MySimpleContract.sol" کلیک کنید.
