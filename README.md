# decimal-group-project
Разработка типа данных - decimal<br/>
Проект включает в себя следующие функции:<br/>

Арифметические операции:

Сложение	+	int s21_add(s21_decimal value_1, s21_decimal value_2, s21_decimal *result)<br/>
Вычитание	-	int s21_sub(s21_decimal value_1, s21_decimal value_2, s21_decimal *result)<br/>
Умножение	*	int s21_mul(s21_decimal value_1, s21_decimal value_2, s21_decimal *result)<br/>
Деление	/	int s21_div(s21_decimal value_1, s21_decimal value_2, s21_decimal *result)<br/>

Операторы сравнения:

Меньше	<	int s21_is_less(s21_decimal, s21_decimal)<br/>
Меньше или равно	<=	int s21_is_less_or_equal(s21_decimal, s21_decimal)<br/>
Больше	>	int s21_is_greater(s21_decimal, s21_decimal)<br/>
Больше или равно	>=	int s21_is_greater_or_equal(s21_decimal, s21_decimal)<br/>
Равно	==	int s21_is_equal(s21_decimal, s21_decimal)<br/>
Не равно	!=	int s21_is_not_equal(s21_decimal, s21_decimal)<br/>

Преобразователи:

Из int	int s21_from_int_to_decimal(int src, s21_decimal *dst)<br/>
Из float	int s21_from_float_to_decimal(float src, s21_decimal *dst)<br/>
В int	int s21_from_decimal_to_int(s21_decimal src, int *dst)<br/>
В float	int s21_from_decimal_to_float(s21_decimal src, float *dst)<br/>

Другие функции:

"Округляет указанное Decimal число до ближайшего целого числа в сторону отрицательной бесконечности"	- int s21_floor(s21_decimal value, s21_decimal *result)<br/>
"Округляет Decimal до ближайшего целого числа"	- int s21_round(s21_decimal value, s21_decimal *result)<br/>
"Возвращает целые цифры указанного Decimal числа; любые дробные цифры отбрасываются, включая конечные нули"	- int s21_truncate(s21_decimal value, s21_decimal *result)<br/>
"Возвращает результат умножения указанного Decimal на -1"	- int s21_negate(s21_decimal value, s21_decimal *result)<br/>

А также тестовые и заголовочныe файлы:<br/>
- compare_func_tests.c<br/>
- converters.c<br/>
- math_funcs_tests.c<br/>
- others_tests.c<br/>
- s21_dec_tests.c<br/>
- s21_dec_tests.h<br/>
- s21_decimal.h<br/>

Для тестирование кода и создания отчета о покрытии - создаются обьектые файлы и статическая библиотека s21_decimal.a
