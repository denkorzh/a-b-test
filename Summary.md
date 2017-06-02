# План-конспект

## Общие положения проверки гипотез
* Гипотезы, ошибки первого и второго рода, significance & power, p-значение
* Критерии хи-квадрат, t-тест, отношения правдоподобия

## Частотный подход
* Схема процедуры, указание на опасность ранней остановки
  - у Ивченко-Медведева в примере 4.2 (стр. 147) рассмотрена биномиальная модель с проверкой гипотезы \theta=\theta_0 против альтернативы \theta = \theta_1 > \theta_0
* Вероятностная модель, как работают сетевые калькуляторы
* **Итого:**
  - лучше всего под эту задачу в обчыном рассмотрении подходит [Welch's t-test](https://en.wikipedia.org/wiki/Welch%27s_t-test)
  - Сумма биномиальных под ЦПТ распределена как сумма нормальных - поэтому используем [вот эти приближения](http://www.machinelearning.ru/wiki/index.php?title=%D0%9A%D1%80%D0%B8%D1%82%D0%B5%D1%80%D0%B8%D0%B9_%D0%A1%D1%82%D1%8C%D1%8E%D0%B4%D0%B5%D0%BD%D1%82%D0%B0#.D0.A1.D1.80.D0.B0.D0.B2.D0.BD.D0.B5.D0.BD.D0.B8.D0.B5_.D0.B4.D0.B2.D1.83.D1.85_.D0.B2.D1.8B.D0.B1.D0.BE.D1.80.D0.BE.D1.87.D0.BD.D1.8B.D1.85_.D1.81.D1.80.D0.B5.D0.B4.D0.BD.D0.B8.D1.85_.D0.BF.D1.80.D0.B8_.D0.BD.D0.B5.D0.B8.D0.B7.D0.B2.D0.B5.D1.81.D1.82.D0.BD.D1.8B.D1.85_.D0.BD.D0.B5.D1.80.D0.B0.D0.B2.D0.BD.D1.8B.D1.85_.D0.B4.D0.B8.D1.81.D0.BF.D0.B5.D1.80.D1.81.D0.B8.D1.8F.D1.85)
* Применение последовательного анализа (http://www.evanmiller.org/sequential-ab-testing.html 
http://www.auduno.com/2014/12/25/rapid-a-b-testing-with-sequential-analysis/ )
  - надо вообще разобраться, что за зверь Sequential Generalized Likelihood Ratio test
  - https://projecteuclid.org/download/pdf_1/euclid.aoms/1177731118 со стр. 164

## Байесовский подход
* https://www.chrisstucchio.com/pubs/VWO_SmartStats_technical_whitepaper.pdf большой подробный обзор
* http://www.exp-platform.com/Documents/2016DSAAcontinuousMonitoringDengLuChen.pdf Нужные вещи о Bayes factors

## Многорукие бандиты
* https://habrahabr.ru/company/ods/blog/325416/
* https://vwo.com/blog/multi-armed-bandit-algorithm/ или почему Бандит хуже с точки зрения VWO
* http://www.cs.mcgill.ca/~vkules/bandits.pdf обзор алгоритмов помимо сэмплирования из статьи Хабра
