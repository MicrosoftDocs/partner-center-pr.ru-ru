---
title: Налог на добавленные значения (НДС) в регистрации центра партнеров
description: Если вам необходимо указать ИДЕНТИФИКАЦИОНный номер плательщика НДС в процессе регистрации центра партнеров, эти сведения помогут вам приступить к работе.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.localizationpriority: medium
ms.date: 10/31/2018
ms.openlocfilehash: 7e4f6778d14166dfe30a608d06dc75d953442c70
ms.sourcegitcommit: d3ff69f285a872fd0a214cc14ac3a6cf9cd124b3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2020
ms.locfileid: "90026483"
---
# <a name="vat-info"></a>Сведения об НДС

**Относится к**

- Центр партнеров
- Коммерческая платформа

Если вы хотите предоставить ИДЕНТИФИКАЦИОНный номер плательщика НДС в процессе регистрации центра партнеров, вот некоторые сведения, которые помогут вам приступить к работе.

## <a name="understanding-vat-numbers"></a>Номера плательщиков НДС

Номер плательщика НДС — это идентификатор, используемый в странах и регионах ЕС. Дополнительные сведения см. в официальном [VIES-сайте](http://ec.europa.eu/taxation_customs/vies/vieshome.do)Европейского союза.

## <a name="accepted-formats-for-vat-numbers"></a>Допустимые форматы номеров НДС

Обратите внимание, что корпорация Майкрософт не предоставляет рекомендаций по налогообложению, и приведенная ниже таблица предоставляется только в качестве руководства. Если это руководство не является достаточным для предоставления корпорации Майкрософт номера НДС, вы должны проверить наличие последних изменений у местных налоговых органов.

<table Responsive="true">
<tr><th>Страна или регион</th><th>Сведения об НДС</th></tr>
<tr><td data-th="Country/region">Австрия
</td><td data-th="VAT info">
<ul>
<li>Формат номера: 1 буква, 8 цифр</li>
<li>Код страны или региона: AT</li>
<li>Пример: U12345678</li>
<li>Примечания. Первый символ — всегда "U".
</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Бельгия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 10 цифр</li>
<li>Код страны или региона: BE</li>
<li>Пример: 1234567890</li>
<li>Примечания. До 1 января 2007 г. использовались 9 цифр.</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Болгария</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 или 10 цифр</li>
<li>Код страны или региона: BG</li>
<li>Пример: 123456789 или 0123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Хорватия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 2 буквы, 11 цифр</li>
<li>Код страны или региона: HR</li>
<li>Пример: HR12345678901</li>
<li>Примечания. Первые символы — всегда "HR".</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Кипр</td><td data-th="VAT info">
<ul>
<li>Формат номера: 2 буквы, 8 цифр, 1 буква</li>
<li>Код страны или региона: CY</li>
<li>Пример: 12345678, 123456789 или 0123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Чехия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 8, 9 или 10 цифр</li>
<li>Код страны или региона: CZ</li>
<li>Пример: 12345678, 123456789 или 0123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Дания</td><td data-th="VAT info">
<ul>
<li>Формат номера: 8 цифр</li>
<li>Код страны или региона: DK</li>
<li>Пример: 12345678</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Эстония</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 цифр</li>
<li>Код страны или региона: EE</li>
<li>Пример: 123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Финляндия</td><td data-th="VAT info">
<ul>
<li>Формат номера: цифр</li>
<li>Код страны или региона: FI</li>
<li>Пример: 12345678</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Франция</td><td data-th="VAT info">
<ul>
<li>Формат номера: 11 цифр</li>
<li>Код страны или региона: FR</li>
<li>Пример: 12345678901, X1234567890, 1X123456789 или XX123456789</li>
<li>Примечания. Может содержать алфавитные символы, за исключением I и Q, в качестве первого или второго символа, а также в качестве первого и второго символа, за которыми следуют 9 цифр.</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Германия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 цифр</li>
<li>Код страны или региона: DE</li>
<li>Пример: 123456789</li>
<li>Примечания. Это должен быть 9-значный цифровой "Umsatzsteur Identifikationnummer" (Ust ID Nr.)</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Греция</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 цифр</li>
<li>Код страны или региона: EL, GR</li>
<li>Пример: 123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Венгрия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 8 цифр</li>
<li>Код страны или региона: DE</li>
<li>Пример: 12345678</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Ирландия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 8 цифр</li>
<li>Код страны или региона: IE</li>
<li>Пример: 1234567X или 1X34567X</li>
<li>Примечания. Включает 1 или 2 алфавитных символа — либо последний, либо второй и последний.</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Италия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 11 цифр</li>
<li>Код страны или региона: IT</li>
<li>Пример: 12345678901</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Латвия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 11 цифр</li>
<li>Код страны или региона: LV</li>
<li>Пример: 01234567890</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Литва</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 или 12 цифр</li>
<li>Код страны или региона: LT</li>
<li>Пример: 123456789 или 012345678901</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Люксембург</td><td data-th="VAT info">
<ul>
<li>Формат номера: 8 цифр</li>
<li>Код страны или региона: LU</li>
<li>Пример: 12345678</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Мальта</td><td data-th="VAT info">
<ul>
<li>Формат номера: 2 буквы, 8 цифр</li>
<li>Код страны или региона: MT</li>
<li>Пример: MT12345678</li>
<li>Примечания. Первые символы — всегда "MT".</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Нидерланды</td><td data-th="VAT info">
<ul>
<li>Формат номера: 11 цифр, 1 буква</li>
<li>Код страны или региона: NL</li>
<li>Пример: 123456789B01</li>
<li>Примечания. Десятый символ — всегда "B".</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Польша</td><td data-th="VAT info">
<ul>
<li>Формат номера: 10 цифр</li>
<li>Код страны или региона: PL</li>
<li>Пример: 1234567890</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Португалия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 цифр</li>
<li>Код страны или региона: PT</li>
<li>Пример: 123456789</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Румыния</td><td data-th="VAT info">
<ul>
<li>Формат номера: 2 буквы, 8-10 цифр</li>
<li>Код страны или региона: RO</li>
<li>Пример: RO12345678, RO123456789 или RO1234567890</li>
<li>Примечания. Первые символы — всегда "RO".</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Словакия</td><td data-th="VAT info">
<ul>
<li>Формат номера: 10 цифр</li>
<li>Код страны или региона: SK</li>
<li>Пример: 1234567890</li>
<li>Примечания. Первые символы — всегда «SI».</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Словения</td><td data-th="VAT info">
<ul>
<li>Формат номера: 2 буквы, 8 цифр</li>
<li>Код страны или региона: SI</li>
<li>Пример: SI12345678</li>
<li>Примечания. Первые символы — всегда «SI».</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Испания</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 цифр</li>
<li>Код страны или региона: ES</li>
<li>Пример: X12345678, 12345678X или X1234567X</li>
<li>Примечания. Включает 1 или 2 алфавитных символа — первый, последний, либо первый и последний.</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Швеция</td><td data-th="VAT info">
<ul>
<li>Формат номера: 12 цифр</li>
<li>Код страны или региона: SE</li>
<li>Пример: 123456789001</li>
<li>Примечания. Последние 2 символа — всегда "01".</li>
</ul>
</td></tr>
<tr><td data-th="Country/region">Соединенное Королевство</td><td data-th="VAT info">
<ul>
<li>Формат номера: 9 или 12 цифр</li>
<li>Код страны или региона: GB</li>
<li>Пример: 123456789 или 123456789001</li>
<li>Примечания. Обычно это 9 цифр, так как 12 цифр обозначают дочернюю компанию группы компаний.</li>
</ul>
</td></tr>
</table>

## <a name="next-steps"></a>Дальнейшие действия

- [Сведения о налогах компании и о том, как добавить или отправить идентификаторы НДС для покупок в центре партнеров](organization-tax-info.md)
