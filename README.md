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
