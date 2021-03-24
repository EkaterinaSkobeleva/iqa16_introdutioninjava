# Отчёт о тестировании Credit Card Number Validator

## Кусок приложения, направленный на проверку валидации номера банковской карты.

24/03/2020 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 1 ч

В результате тестирования выявлены следующие дефекты:
* не выявлены


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* наработка кода для валидации номера банковских карт
* ресурс https://www.freeformatter.com/credit-card-number-generator-validator.html для генерации случайных номеров банковских карт


В качестве тестовых данных использовались данные (источник даннх https://www.freeformatter.com/credit-card-number-generator-validator.html):
* number = "5351719427810741"  Result is ОК 
* number = null  Result is FAIL
* number = "1122 2222 2234 2421"   Result is FAIL
* number = "1122222222342421"   Result is OK
* number = "112222222234"   Result is FAIL
* number = "11222222223424215"   Result is FAIL 
* number = "4556284756383485"   Result is OK 
* number = "0556284756383485" Result is FAIL 
* number = "9556284756383485" Result is FAIL
* number = "asdf284756383485" Result is FAIL
* number = "9pdf284756383485" Result is FAIL
* number = "2221005065877662" Result is OK
* number = "373379189006783" Result is FAIL
* number = "6011047780845348" Result is OK
* number = "3528483915531318" Result is OK
* number = "5537251900061797" Result is OK
* number = "30276747541969" Result is FAIL
* number = "36106571338956" Result is FAIL
* number = "6759933838290189" Result is OK
* number = "4026690571488139" Result is OK
* number = "6376305905614844" Result is OK

Тестирование производилось в следующем окружении:
* Windows 10, x64
* OpenJDK11U-jdk_x64_windows_hotspot_11.0.10_9
* IntelliJ IDEA Community 2020.3.3