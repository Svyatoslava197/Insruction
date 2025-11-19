# Instruction

## Пункт 1. В инструкции Александра:

- Заходи на сайт https://renode.io/
- Нажимаем на кнопку "Get Started" или переходим по ссылке: https://renode.io/#downloads

 **Выполнено успешно**

![image](https://github.com/user-attachments/assets/2696d94a-3892-4131-ab23-ec05149dc235)

![image](https://github.com/user-attachments/assets/47fb8606-2b18-4662-823a-1b93a4d77239)

## Пункт 2. "Настраиваем C/C++ для Visual Code" - выполнен

### Установка компилятора

Компилятор - это программа, которая переводит ваш код с языка C на "язык микроконтроллера" (машинный код).

**Файл для скачивания:**

![image](https://github.com/user-attachments/assets/e5d690ef-5392-4a20-b769-ead65ddea5b6)

**Более подробное описание установки:**

**Процесс:**
1. Скачали MinGW-w64 с winlibs.com - это набор инструментов включая GCC
2. Распаковали в `C:\mingw64` - создали "дом" для компилятора

![image](https://github.com/user-attachments/assets/242e700e-a3a5-40e7-815d-78c41f17bd5c)

3. Добавили в PATH - сказали системе "где искать компилятор"

![image](https://github.com/user-attachments/assets/521d7438-f4a7-46b1-859f-e6918b5c108a)

4. Проверили командой `gcc --version`
5. Установила расширение в Visual Code

![image](https://github.com/user-attachments/assets/c426e4a0-d54c-491f-bb26-9ef0d483725c)

![image](https://github.com/user-attachments/assets/3175929e-9eb8-4f66-9f4b-7ec4beffde19)

## Пункт 3. "Меняем json в компиляторе C"

**Создание папки проекта**

![image](https://github.com/user-attachments/assets/05d8d621-b006-47ef-8aa6-71fee368871d)

Создала файл `c_cpp_properties.json` - это "инструкция" для VS Code

![image](https://github.com/user-attachments/assets/115513a4-9304-4597-9eca-c24a28753cce)

## Пункт 4. Написание кода для STM32

- Создала файл `stm32_program.c`
- Добавила код для работы с регистрами STM32
- Скомпилировала в .bin формат

**Команды компиляции:**

C:\mingw64\mingw64\bin\gcc.exe -nostdlib -ffreestanding -O0 -c stm32_program.c -o stm32_program.o
C:\mingw64\mingw64\bin\objcopy.exe -O binary stm32_program.o stm32_program.bin


![image](https://github.com/user-attachments/assets/f404601f-3b9d-41c9-a2d3-b20e66b022dc)




