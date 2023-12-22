<table border="1" width="100%" cellpadding="40" cellspacing="10"><tbody>
  <tr>
    <td width="20%" align="center">
      <img src="pic/kandinsky-download-1697056680849.png" height="150" width="150">
    </td>
    <td valign="top">
      <h3>Прогнозирование температуры расплава стали после окончания стадии легирования</h3>
      <br><i>Forecasting the Steel Melting Temperature at the End of the Alloying Stage</i>
    </td>
  </tr>
  <tr>
    <td valign="top">
      <a title="Использовать для просмотра Jupyter nbviewer" href="https://nbviewer.org/github/georgiy-vasilevskiy/test_repo/blob/main/Forecasting_the_Steel_Melting_Temperature_at_the_End_of_the_Alloying_Stage.ipynb">
        <img src="https://img.shields.io/badge/Смотреть-ipynb-F37626">
      </a>
      <a title="Использовать для просмотра GitHub & BitBucket HTML Preview" href="https://htmlpreview.github.io/?https://github.com/georgiy-vasilevskiy/test_repo/blob/main/Forecasting_the_Steel_Melting_Temperature_at_the_End_of_the_Alloying_Stage.html">
        <img src="https://img.shields.io/badge/Смотреть-html-54B231">
      </a>
    </td>
    <td>
      <b>Ключевые слова:</b> предобработка данных, описательный анализ, корреляционный анализ, машинное обучение, формирование набора данных для обучения алгоритмов, MAE
    </td>
  </tr>
</tbody></table>

Современное производство стали использует большое количество электрической энергии. Большая её часть идёт на нагрев и плавление сырья и вспомогательных реагентов, а также на поддержание температуры расплава на заданном уровне. Снижение уровня потребления электроэнергии позволит снизить расходы на неё, что приведёт к сокращению затрат на производство стали, снижению её себестоимости и, как следствие, повышению конкурентоспособности продукции металлургического предприятия.

**Исходные данные:** сведения о параметрах стадии легирования. Для каждой выпускаемой партии стали доступны сведения о поданных легирующих добавках, инертном газе, работе электродах и результатах измерения температуры.

**Цель проекта:** построить модель, прогнозирующую температуру расплава стали после окончания стадии легирования.

**Инструменты:** pandas, os, re, matplotlib, seaborn, scikit-learn, catboost, lightgbm, xgboost.

**Результаты исследования**

Наилучшие показатели качества демонстрирует модель регрессии LASSO с максимальным числом итераций — 1000, альфой — 0,1 и порогом остановки обучения — 0,00001, с зафиксированной псевдослучайностью (random_state=250923), обученная на масштабированных данных. Значение MAE, полученной в результате проведения кросс-валидации, равно 6,1 ∘C. Значение MAE на тестовой выборке равно 5,9 ∘C.

 ![visitors](https://visitor-badge.laobi.icu/badge?page_id=georgiy-vasilevskiy.test-repo)


![](https://komarev.com/ghpvc/?username=georgiy-vasilevskiy&label=Profile+views)

