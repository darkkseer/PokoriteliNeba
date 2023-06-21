# Команда Покорители неба 

## Аппаратная часть
**В качестве вычислетельно модуля мы будем сипользовать _Raspberry Pi 4_. Фотографии будут совершаться с помощью _Raspberry Pi Camera_, глабоальные координаты считываться с помощью _GPS-модуля_**

![Pipeline (1)](https://github.com/darkkseer/PokoriteliNeba/assets/92098618/48c776a9-bebd-485d-8a4f-c25d6dd0db68)

**Также на фото предствлены команды, с помощью которых будут общеться модули. С камеры будут послаться фото, а с GPS-модуля текущие координаты самолета на микрокомпютер. Далее будет происходить детекция армянских символов, если такой был обнаружен, записываем данные на SD-карту.**


## Программная часть
**Програмная часть будет реализована на языке Python**

![Pipeline (2)](https://github.com/darkkseer/PokoriteliNeba/assets/92098618/d93b5f33-fb27-4162-8adc-85f6b358aed2)

### Описание функции _detection()_

**С помощью фреймворка OpenCV будет реализована предобработка изображения: детекция белого прямогульника, обрезание фото и применение световых фильмов для большей читаемости символа**

**Для распознания армянских символов будет использоваться нейронная сеть _OCR_. С помощью API будут пробрасываться предобработанные данные. Если символ распознан - записываем его на карту. Повторяем данный цикл до конца окончания полета.**

## Демонстрация предобработки

**Исходное изображение**

![image](https://github.com/darkkseer/PokoriteliNeba/assets/92098618/d4f2a618-e246-40a3-a23e-43cbd6d0e73a)

**Обрезанное и обработанное изображение**

![image](https://github.com/darkkseer/PokoriteliNeba/assets/92098618/9a047947-5850-4991-a77f-37859d0d4641)





 
