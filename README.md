
# Отчеты
<details>
  <summary>Инструкция по редактированию отчетов в ERP</summary>
  
[Инструкция по редактированию отчетов в ERP](Инструкции/ERP/Инструкция%20по%20редактированию%20отчетов%20ЕРП.pdf)
  
</details>
<details>
  <summary>Выпуск продукции из перемещения</summary>
  
[Описание](Отчеты/Выпуск%20продукции%20из%20перемещения.md)
  
</details>

# Обработки
# ERP
<details>
  <summary>Номенклатура</summary>

  [Разбитие номенклатуры на составляющие](ERP/Расширения/ГенерацияНоменклатуры/ОбщиеМодули/ПолучитьДанныеИзНоменклатуры.md)    

</details>
<details>  
  <summary>Продажи</summary>

  <details>
  <summary>Заказы клиентов</summary>
    
[Проверка стоимости позиций заказа клиента при печати спецификации](ERP/Расширения/ВсёВОдном/ЗаказКлиента.ФормаДокумента.md#функция-проверкацены)   
[Приведение к Цене за км](ERP/Расширения/ВсёВОдном/ЗаказКлиента.ФормаДокумента.md#процедура-всеводномзапретпесчетаценприизменениипослеэлемент)  
</details>
</details>
<details>  
  <summary>Производство</summary>

  <details>
  <summary>Заказы на производство</summary>
    
[Добавление IDZak в заказ клиента](ERP/Расширения/ВсёВОдном/ЗаказНаПроизводство.МодульОбъект.md)  
</details>
<details>
  <summary>Паспорта КПП</summary>
    
[Создание контроля веса](ERP/Расширения/СертификатыНаКабель)  
</details>
<details>
  <summary>Контроль веса КПП</summary>
</details>
</details>

<details>
  <summary>Контроль продукции</summary>

  <details>
  <summary>Контроль продукции</summary>
    
  [Нахождение по IDZak длинны намотки в КП](ERP/Расширения/КонтрольПродукции/КП.МодульОбъекта.md)
  
</details>
</details>

# Expert V
<details>
  <summary>ЦПМ</summary>

  ## ШиныЦПМ
  
  ## НомерКристализатора

  ## ЦПМ Фильера

  ## Номенклатура оборудований ЦПМ
  
  ## Номенклатура оборудований ЦПМ

  ## Признак сырья
  <details>
  <summary> ЦПМ документ (выработка) </summary> 
   
  [Заполнение Сменного задания](EV/ЦПМДокумент.ФормаЭлемента.md)
  </details>

  ## Оптимальное размещение продукции ЦПМ
  <details>
    
  [Сгруппированные заказы склад](EV/СгруппированныеЗаказыСклад)
  
  [Сменное задание упаковки шин](EV/СменноеЗаданиеУпаковкиШин)
  </details>
    
</details>


<details>
  <summary>ЦКПП</summary>
  <details>
  <summary> Сгруппированные заказы </summary> 

  [Актуализация Сгруппированных заказов с Excel](EV/Сгруппированные%20заказы/ФормаСписка.СинхронизацияСExcel.md)
         
  </details>  
  
  <details>
  <summary> Шахтная Производительность оборудования </summary> 

  [Шахтная Производительность оборудования](EV/Общие%20Модули/РасчетПроизводительностиОборудований.md?plain=1#L1)
 
  [КодФуРасМат](EV/Общие%20Модули/Формирование%20рабочих%20массивов.md?plain=1#L483)
         
  </details>  
</details>
  
  
  
  </details> 

  </details> 

# Expert V <-> ERP
<details>
  <summary>Создание заказа из ERP</summary>
  
  [Отправка заказа из ERP](ERP/Расширения/ВсёВОдном/ЗаказНаПроизводство.МодульОбъект.md?plain=1#L9)
  
  [Принятие заказов в EV](EV/HTTP-сервисы/Заказы.md?plain=1#L1)
     
  [Создание документа в EV](EV/Общие%20Модули/Формирование%20рабочих%20массивов.md?plain=1#L1)

</details>

<details>
  <summary>Пометка удаления заказов EV при пометке на удаление заказа на производство в ERP</summary>
  
  [Запрос на удаление из ERP](ERP/Расширения/ВсёВОдном/ЗаказНаПроизводство.МодульОбъект.md?plain=1#L33)

  [Пометка на удаление в EV](EV/HTTP-сервисы/ЗаменаСтрокЗаказов.md?plain=1#L58)
  
</details>

<details>
  <summary> Создание спецификации </summary>
  
  [Создание спецификации в ERP](/ERP/Расширения/СпецификацияРасширение/Ресурсная%20спецификация/Форма%20элемента.md?plain=1#L1)
  
  [Запросы на заполнение из ERP (Факт)](ERP/Расширения/СпецификацияРасширение/Заказ%20на%20производство%20.%20Форма%20документа.md?plain=1#L22)
  
  [Запросы на заполнение из ERP (Эталон)](/ERP/Расширения/СпецификацияРасширение/Ресурсная%20спецификация/Форма%20элемента.md?plain=1#L54)
  

</details>

<details>
  <summary> Создание и заполнение этапа/производственного процесса </summary>
  
  Этап = Производственный процесс
  
  [Создание первого этапа](ERP/Расширения/СпецификацияРасширение/Ресурсная%20спецификация/Форма%20элемента.md?plain=1#L297)
  
  [Создание второго этапа](ERP/Расширения/СпецификацияРасширение/Ресурсная%20спецификация/Форма%20элемента.md?plain=1#L332)
  

</details>

<details>
  <summary> Создание ПБЗ и Сборки в ERP из EV </summary>
  

  [Создание ПБЗ и Сборки в ERP](ERP/HTTP-сервисы/Всё%20в%20одном.auto_pbz.md?plain=1#L49)
  
  [Запрос на создание ПБЗ и Сборки из EV](EV/Общие%20Модули/Ерп%20обмен.md?plain=#L11)
  

</details>
      
      



