[Условие](https://github.com/ZhMax/basic_sparse_quant/tree/main/notebooks)

## Домашняя работа часть 1 (5 баллов): анализ падения точности LLM после квантизации и спарсификации


В этом задании вам предстоит проанализировать несколько методов компресии больших языковых моделей, в частности методы QUIK, Wanda и SparseGPT.

В качестве модели будет использована модель opt-350m.

Результат задания: Построить три графика (для каждого датасета) зависимость точности модели от уровня сжатия (квантизации или спарсификации).

В виде решения нужно будет сдать ноутбук с построенными графиками и выводами, в частности ответить на вопрос что маштабируется лучше и какой метод спарсификации выбрать.



## Домашняя работа часть 2 (5 баллов): совмещение спарсификации и квантизации.


В этом задании вам предстоит совместить спарсификацию и квантизацию в рамках фреймоврка OBS.
Метод самой квантизации может быть любым.


Что бы упросить задание, мы не будем квантизовать всю модель, а квантизуем только по слоям.

Резальтат работы это метрики L1 и L2 для $|C(W)X^T - WX^T|$ для каждого слоя, $С$ функция спарсификации и квантизации.


В папке llama7b_weights содержатся веса для одоного слоя LLaMа7b и сопутствующие активации в папке llama7b_act_scales (аггрегировые по датасету)




### Оба задания сдаются в виде ноутбуков с решением


## Домашняя работа засчитана если вы набираете 7 баллов.