# ГЛАВА 1

## Многоуровневая компьютерная организация

### Языки, уровни и виртуальные машины

**Я0** - Встроенные машинные команды 
**Яn** - язык уровня
**Mn** - Виртуальная машина 

**Первый способ** - программы, написанной на языке Я1, подразумевает замену каждой команды эквивалентным набором команд на языке Я0.
Компьютер исполняет новую программу, написанную на языке Я0. Эта технология называется трансляцией.

**Второй способ** заключается в создании на языке Я0 программы, получающей
в качестве входных данных программы, написанные на языке Я1. При этом каждая команда языка Я1 обрабатывается поочередно, после чего сразу исполняется эквивалентный ей набор команд языка Я0. Это  называется интерпретацией, а программа, которая осуществляет интерпретацию, называется интерпретатором.


**Уровень n** [Яn, Мn] {Интерпритируются на Мn-x (более низкого уровня), либо трагслируются в Яn-x(более низкого уровня)}
**Уровень 2** [Я2, М2] {Интерпритируются на М1/М0, либо трагслируются в Я1/Я0}
**Уровень 1** [Я1, М1] {Программы выполняются интерпитатором или транслируются на Я0}
**Уровень 0** [Я0, М0] {Программы выполняются электроными схемами}
**Уровень ФИ** {Уровень физических устройств}

### Современные многоуровневые машины

**Уровень 5** - Уровень языка прикладных программистов (Языки высокого уровня)
>               |
>               v
>      [Трансляция(Компилятор)]
>               |
>               v
**Уровень 4** - Уровень Ассемблера (Язык Ассемблера)
                |
                v
        [Трансляция(Компилятор)]
                |
                v
**Уровень 3** - Уровень ОС (новый набор команд, другая организация памяти, способность исполнять две и более программ
одновременно и некоторые другие)
                |
                v
    [Частичная интерпритация(ОС)]
                |
                v
**Уровень 2** - Уровень архитектуры набора команд (машинные команды)
                |
                v
    [Интерпритация(микропрограмма)]
                |
                v
**Уровень 1** - Уровень микроархитектуры (АЛУ|арифметико-логическое устройство, 8/32 регистра формируют локальную память и схему)
                |
                v
        [Аппаратное обеспечение]
                |
                v
**Уровень 0** - Цифровой логический уровень (вентили)

> Машинные языки уровней 1, 2 и 3 — цифровые


транзисторы -> вентили -> биты -> регистры -> арифметико-логические устройства

> важно запомнить, что компьютер проектируется как
> иерархическая структура уровней, которые надстраиваются друг над другом.
> Каждый уровень представляет собой абстракцию некоторых объектов и операций.

**Набор типов данных, операций и характеристик каждого отдельно взятого
уровня называется архитектурой**

### Развитие многоуровневых машин

Аппаратное обеспечение состоит из материальных объектов — интегральных схем, печатных плат,
кабелей, источников электропитания, модулей памяти и принтеров

Программное обеспечение, состоит из алгоритмов (подробных последовательностей команд, которые описывают решение некоторой задачи) и их компьютерных представлений - программ

> Аппаратное и программное обеспечение логически эквивалентно.
