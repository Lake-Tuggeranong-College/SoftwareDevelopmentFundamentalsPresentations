---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
# backgroundImage: url('https://camo.githubusercontent.com/34308662b9bab4db034673cec18b6ca3893069700cf7f135b06f60c4246f645b/68747470733a2f2f79686174742d6d6172702d636c692d6578616d706c652e6e65746c6966792e636f6d2f6173736574732f6772616469656e742e6a7067')
---

![bg left:40% 80%](https://www.php.net/images/logos/new-php-logo.svg)

# **Software Development Fundamentals**

Website Development - PHP

---

# Course Structure

- This course uses the generic, language agnostic ```Software Development Fundamentals``` course as a base. 


- The Fundamentals course will introduce the topics / concepts for each stage, and this page has the language / platform specific implementation.

- General broad knowledge, specific skills

---

![bg center w:900](./images/GeneralProgrammingSkills.png)

---

# What is Programming?

- Executing (running) code
- The programmer writes high level language.
- Compiler / Interpreter converts it to Hardware
![bg right 100%](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/8e821c51-d615-412e-8580-08fc5c123c16/DE3905E0-7D18-4473-98B8-1E60725FF556.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221103%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221103T033634Z&X-Amz-Expires=86400&X-Amz-Signature=607f146026e88808abef7b922e05a9de87ae995e3b2ca14248f7f9ae2883a95a&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22DE3905E0-7D18-4473-98B8-1E60725FF556.png%22&x-id=GetObject)

---
# Syntax
```
# Python
print("Hello World")
```

```
// Arduino
Serial.println("Hello World");
```

```
PHP
<?php
echo "Hello World!";
?>
```
---
# Syntax
```
Assembly - x86 32 bit Mac OSX

global start
section .text
start:
    push    dword msg.len
    push    dword msg
    push    dword 1
    mov     eax, 4
    sub     esp, 4
    int     0x80
    add     esp, 16
    push    dword 0
    mov     eax, 1
    sub     esp, 12
    int     0x80

section .data
msg:    db      "Hello, world!", 10
.len:   equ     $ - msg
```
--- 
# Executing Code

Depending on the language and environment, there are two broad approaches to executing code - **interpreted** and **compiled**.

- **Interpreted** code is executed line by line by the interpreter.

- **Compiled** code is when the compiler analyses the entire code, checks for errors and then produces an executable

--- 
# Interpreted vs Compiled

Neither is *better*, it depends on the circumstances. 

|Compiled | Interpreted|
|---|---|
|can take time to compile the entire code base before it can execute| can allow for more flexible programming|
|once the code is running, it is generally faster.|tend to execute slower than compiled languages|

---
## Input Processing Output

Most parts of code comprise of three things:
- Input
    - User name, Mouse clicks etc.
- Processing
    - Converting data from input into desired output, etc.
- Output
    - Result of calculation, writing to a database etc.
---

![bg 75%](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2194f8be-cb46-4b16-b8a8-39b1b941c545/6F444F51-80BC-4F3E-BFE8-E1869D084D5D.jpeg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221103%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221103T035854Z&X-Amz-Expires=86400&X-Amz-Signature=07846c74cc01c764de14183a408c83e16205e8f077520aa698d8fc2173d449bd&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%226F444F51-80BC-4F3E-BFE8-E1869D084D5D.jpeg%22&x-id=GetObject)

---
# Key Terms

|Term|Definition|
|--|--|
|IDE|Integrated Development Environment. The program used to code, which typically provides the developer different tools to assist the development process - not just a text editor.|
|Programming|Giving instructions to the computer to execute.|

---
# Choose Your Path

[![h:100](./images/logoArduino.png)](#13) Robotics 
[![h:100](./images/logoPHP.png)](#14) Website Development (Odd years)
[Python](#13) Website Development (Even Years)
[GDScript](#13) Interactive Software Development 



---
# Arduino

NOTE!

Arduino refers to the IDE, Language AND the board!

---
# Arduino 2

---

# PHP