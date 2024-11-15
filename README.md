# Задача о разборчивой невесте


| Гаев Роман | 209М |
| --- | --- | 
| Лавренченко Мария | 209М |
| Панцырный Иван | 214М |
| Орачёв Алексей | 209М |


## Описание
- Невеста ищет себе жениха (существует единственное вакантное место).
- Число претендентов - N.
- Невеста общается с претендентами в случайном порядке, с каждым не более одного раза.
- О каждом претенденте известно, лучше он или хуже любого из предыдущих.
- Пообщавшись с претендентом, невеста сравнивает его с предыдущими и либо отказывает, либо принимает его предложение. Если предложение принято, они женятся и процесс останавливается. Если невеста отказывает жениху, то вернуться к нему позже она не сможет.
- Невеста выигрывает, если она выберет самого лучшего претендента. Выбор даже второго по порядку сравнения — проигрыш.

## Задача
- Разработать и обучить нейронную сеть, которая возьмет на себя роль невесты и будет решать принять предложение или отказать очередному жениху.
- Сравнить результат принятия решения обученной нейронной сети и оптимальным математическим алгоритмом.

## Решение
- RL алгоритм PPO из stable_baselines3
- RL алгоритм DQN из stable_baselines3
- Правило 37

| Метод | % | кол-во шагов | время обучения |
| --- | --- | --- | --- |  
| PPO | 37.06% | 500000 | 5м 35с |
| DQN | 32.41% | 500000 | 3м 22с |
| Правило 37 | 37.05% | --- | --- |


| Кривая обучения DQN | Кривая обучения PPO |
| --- | --- | 
| ![График](https://github.com/Dr1MTeam/RL_Secretary/blob/main/resources/36d0de58-27b3-4891-97c8-e3c1b5a3f005.png) | ![График](https://github.com/Dr1MTeam/RL_Secretary/blob/main/resources/15b510ed-56dc-43cf-bc19-6e218121112c.png) | 

