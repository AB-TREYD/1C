 ## Функция new_spec(Запрос)

<details>  <summary>     Код  </summary>

	// тут мы получаем новую спецификацию
	СервисОтвет = Новый HTTPСервисОтвет(200);   
	// тут мы получаем новую спецификацию
	Перезаполнение_из_хттп_Сервиса  =?(Запрос.ПараметрыЗапроса.Получить("a")="Да",Истина,Ложь);
	Структ = РаботаСоСпецификацией.ОбработатьФайлик_new_spec(РаботаСоСпецификацией.ФормированиеТЗ_new_spec(),1);
	РаботаСоСпецификацией.ЗаполнитьСпецификацию(Структ.ТЗ,Структ.IDZAKAZA,Структ.Признак);		
	
	Структ2 = РаботаСоСпецификацией.ОбработатьФайлик_new_spec(РаботаСоСпецификацией.ФормированиеТЗ_new_spec(),2);
	Если Структ2.Признак = "Эталон" тогда Структ2.ТЗ.Колонки.КоличествоУпаковок.Имя = "ЭталонныйНорматив" КонецЕсли;      	
	РаботаСоСпецификацией.ЗаполнитьСпецификацию(Структ2.ТЗ,Структ2.IDZAKAZA,Структ2.Признак);		
	
	
	Если Перезаполнение_из_хттп_Сервиса тогда  //Сюда попадет только при отправке из EV
		Документ = РаботаСоСпецификацией.ПолучитьДок(Структ.БЗ,Структ.IDZAKAZA);   
		Если Документ <> неопределено тогда
			РаботаСоСпецификацией.ВписатьСпецификациюВДокумент(Документ,Структ.БЗ);       
		
  ## #ОБласть Только_ПБЗ_код
  <details> 
    
			//ТУТ ТОЛЬКО ПБЗ
			Если Структ.БЗ и Структ.Отходы и Структ.Признак = "Производственная" тогда 		//ТУТ всегда ПБЗ!				
				Документ = Документ.ПолучитьОбъект();                                                                   
				Документ.Перезаполнение_из_хттп_Сервиса = Истина;
				РаботаСоСпецификацией.ДополнитьПоСпецификацииДляПБЗ(Документ);
				Документ.Записать();
			КонецЕсли;	
		КонецЕсли;	
	КонецЕсли;	
	
  </details>  
  
	Возврат СервисОтвет;
</details>  
