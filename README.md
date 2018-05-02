## Задача
Используя имеющиеся исторические данные, реализовать прототип торговой стратегии, провести backtest (учитывая transaction costs), оценить результат.
Класс стратегий и используемый инструментарий могут быть любыми.

**keywords:** `machine_learning`, `deep_learning`, `data_mining`, `survivorship_bias`, `data_snooping`
<br><br>

## Возможные варианты стратегий
#### Pairs Trading (mean reversion):

Используя статистические тесты, раз в период осуществлять поиск коинтегрированных пар/троек активов вида:
<p align="center"><img src = "http://latex.codecogs.com/gif.latex?%5Cbeta%20_1%5Ctimes%20A_1&amp;plus;%5Cbeta%20_2%5Ctimes%20A_2&amp;plus;%5Cbeta%20_3%5Ctimes%20A_3%20-%20%5Cmu"/></p>

Учитывая свойство возврата к среднему формировать динамический портфель из найденных комбинаций. Оценка текущего режима волатильности может быть использована, как фактор масштабирования размер позиции. 


**keywords:** `cointegration`, `stationarity_test`, `johansen_test`, `augmented_dickey_fuller_test`
<br><br>
#### Basket Trading:
Используя list- или pairwise подход, раз в период решать задачу ранжирования акций, входящих в индекс S&P500. На основе полученного ранкинга формировать рыночно-нейтральный портфель. Ранжирование можно осуществлять внутри отдельных секторов.

**keywords:** `learning_to_rank`, `pointwise`, `pairwise`, `listwise`, `RNN`, `LSTM`

Языки программирования: Python, R