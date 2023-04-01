## Символы и генераторы
[![Build status](https://ci.appveyor.com/api/projects/status/uf355gyus8mm1koo?svg=true)](https://ci.appveyor.com/project/Pavka16/symbols-and-generators)
---

### Легенда

Реализовывать итераторы не так уж просто. Давайте посмотрим, как при переборе вам могут помочь генераторы.

### Описание

В этом задании предполагается, что все персонажи содержат набор полей:
```javascript
{
  name: 'Лучник',
  type: 'Bowman',
  health: 50,
  level: 1,
  attack: 40,
  defence: 10
}
```

Используйте заготовку для организации перебора класса `Team`:
```javascript
class Team {
  ...
  *[Symbol.iterator]() {
    // это генератор
    // и здесь есть доступ к this
    // остаётся лишь правильно написать yield
  }

}
```