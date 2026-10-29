<p align="center">
  <img alt="Windows 10/11" src="https://img.shields.io/badge/Windows-10_11-0078D7?style=flat-square&logo=windows&logoColor=white" />
  <img alt="Linux x86_64" src="https://img.shields.io/badge/Linux-x64-F5C518?style=flat-square&logo=linux&logoColor=black" />
  <img alt="Android ARM64" src="https://img.shields.io/badge/Android-ARM64-3DDC84?style=flat-square&logo=android&logoColor=white" />
  <img alt="Windows 7 legacy" src="https://img.shields.io/badge/Windows_7-legacy-6C757D?style=flat-square&logo=windows&logoColor=white" />
</p>

<h1 align="center">🌩️ Индра</h1>

<p align="center"><strong>Индра правит сетью: Tor вместо VPN.</strong><br/>
Запустил — интернет через Tor. Выключил — как было.<br/>
Ничего прописывать руками не нужно, аккаунт и облако не нужны.</p>

<div align="center">

[![Windows — Download](https://img.shields.io/badge/Windows-Download-0078D7?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/lightclove/indra-releases/releases/latest)
[![Linux — Download](https://img.shields.io/badge/Linux-Download-F5C518?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/lightclove/indra-releases/releases)
[![Android — Download](https://img.shields.io/badge/Android-Download-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/lightclove/indra-releases/releases)
[![Windows 7 — Download](https://img.shields.io/badge/Windows_7-Download-6C757D?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/lightclove/indra-releases/releases/tag/indra-win7)

</div>

Здесь **готовые файлы**. Исходников нет.

---

## 🎯 Что качать

Одна строка вместо паники: **качай файл своей системы, остальное пропускай.**

| Ты на… | Качай | Где на странице релизов |
| ------ | ----- | ----------------------- |
| 💻 Windows 10 / 11 (64 бит) | `indra_…_….zip` | релиз **«Индра … — Windows»**, помечен `Latest` |
| 🐧 Linux x86_64 | `indra_…-x86_64.AppImage` | релиз **«Индра … — Linux»** |
| 📱 Android (ARM64) | `mindra_…_….apk` | релиз **«Индра … — Android»** |
| 🪟 Windows 7 (64 / 32 бит) | `indra_…-win7.zip` | релиз **«Индра … — Windows 7»** |

> ⚠️ Внизу каждого релиза GitHub сам лепит **«Source code (zip)»** и
> **«Source code (tar.gz)»**. Это не Индра — внутри просто текст этой
> страницы. Не качай их.

---

## 🧭 Три уровня сборок

Сверху вниз на странице релизов идут три уровня. **Для обычного использования бери средний — стабильный.**

| Уровень | Пометка | Кому |
| ------- | ------- | ---- |
| 🧪 **Предпросмотр** (alpha) | `Pre-release`, выше всех | Хочешь новое раньше и готов мириться с багами |
| ✅ **Стабильный** | `Latest`, в середине | **Тебе, по умолчанию** |
| 🗂 **Архив** | ниже всех | Осознанный откат на прежнюю версию |

Метка `Latest` стоит на одном стабильном релизе (сейчас — Windows) и не значит
«единственно правильный»: Linux и Android качай из своих стабильных релизов рядом.

---

## 🤔 Зачем

VPN платный, серверы режут, клиент тяжёлый. Tor Browser — отдельный браузер:
Chrome, Edge, Telegram и приложения на телефоне сами через него не идут.

Запустил — интернет через Tor. Выключил — как было. Сеть уже есть, свои серверы
не нужны; в жёсткой фильтрации помогают мосты; архив можно отдать без магазина
и аккаунта.

Это не коммерческий VPN. Трафик идёт через сеть добровольцев Tor. Сайт видит
адрес выходного узла, не ваш домашний.

<details>
<summary>🚫 Чего ждать не стоит</summary>

- Кто сидит рядом, видит экран.
- Вошли логином — сайт знает, что это вы; не знает только домашний адрес.
- Откроется не всё: часть сайтов режет адреса Tor.
- Через Tor обычно медленнее, чем напрямую.
- Это не антивирус.

Нужен быстрый канал до своего сервера — другая программа.

</details>

---

## ▶️ Как запустить

- **Windows.** Распакуй архив целиком, дважды нажми программу. Файлы по разным
  папкам не разбрасывай.
- **Linux.** Один файл: в свойствах разреши запуск и открой. Двойной клик — то же
  окно, что на Windows. Нет графики — сеть поднимется в терминале. Не открылся:
  `APPIMAGE_EXTRACT_AND_RUN=1 ./indra_….AppImage`.
- **Android.** Открой apk. Подпись не из магазина — система один раз спросит.
  Дальше иконка **Indra**, не исходный файл. При включении нужен системный VPN,
  иначе приложения пойдут мимо Tor. Нужен 64-битный ARM (обычные телефоны
  последних лет).

Выключить: на компьютере крестик на левом виске морды или Escape; на телефоне —
то же касание, которым включал, или системный ключ VPN.

ПК выключил «на горячую» — при следующей загрузке Windows Индра попытается
откатить настройки сама.

Подожди, пока не будет видно, что выход есть. Потом браузер как обычно.

Антивирус съел файлы рядом с программой — частое ложное срабатывание на Tor:
карантин, исключения.

---

## ✨ Что умеет

На компьютере системный прокси: Chrome, Edge и кто его слушается идут через Tor.
На телефоне прокси приложения игнорируют — поднимается системный VPN.

**Telegram** на компьютере настройки на лету часто не берёт. Если уже был открыт,
пока Индра поднимался, процесс не убиваем — шестерёнка или меню «Параметры» →
«Перезапустить Telegram» (не во время звонка). Был закрыт — открой после «готово».
На телефоне идёт через VPN вместе с остальными.

**Мосты** включены сами. Прямой вход режут — другой порядок, свежий список, потом
запасные каналы под обычный просмотр сайтов. Отдельный «уже свободный» интернет
не нужен.

**Обновление.** Шестерёнка (на телефоне — меню) → «Обновить», когда сеть уже жива.
Настройки не затираются. Пока выключен, кнопка: «сначала открой врата». На компьютере
движок Tor рядом подтягивается сам, когда выход есть; на телефоне новый Tor приходит
вместе с новым apk. Сама программа «вышла версия» не пишет.

**Страна выхода** — в шестерёнке или в меню: конкретная страна или «любой».
Запоминается.

**Логи.** Первый запуск окна: язык и писать ли журнал на диск. Без согласия на диск
ничего лишнего. Зависло: компьютер — шестерёнка → «Снять логи» (архив на стол);
телефон — меню → «отправить логи». Этот файл в [Telegram](https://t.me/lightclove),
а не «опять завис».

Слушает только твой компьютер или телефон. При выходе настройки возвращает.
Аккаунта и облака нет.

<details>
<summary>🩹 Если не так</summary>

**Долго собирает цепь.** Режут прямые входы. Подожди, особенно на мобильном
интернете. Мосты и запасной канал переберутся сами.

**Сайт есть, Telegram на компьютере нет.** Уже был открыт — «Перезапустить
Telegram». Был закрыт — открой после «готово».

**После выключения всё ещё через прокси.** Выключи ещё раз. На Windows после
перезагрузки есть страховка.

**Сайт не открылся после «готово».** Часть сайтов режет выходные адреса Tor.
Цепь при этом может быть жива.

**Помощь.** Сними логи, воспроизведи, пришли архив: [Telegram](https://t.me/lightclove).

Вы отвечаете за то, как пользуетесь сетью. Это тот же Tor, что у официального браузера.

</details>

---

## 📛 Откуда имя

В «Ригведе» Индра — не абстрактный «громовержец», а рабочий царь: до боя пил сома,
после — бил. Его ваджру выковал божественный кузнец Тваштар, а когда оружие не взяло
змея Вритру — перековали из костей мудреца Дадхичи, который отдал их добровольно.
Само имя «Вритра» означает «заслон»: змей не жёг и не грабил — он просто лёг на воды
и закрыл источник.

Здесь воды — интернет, заслон — всё, что лежит на канале: реестр, DPI, «ваш регион»,
школа, офис — не только РКН. Ваджра — эта программа рядом с официальным Tor.

---

## 📖 Словарь терминов

Незнакомое слово в интерфейсе: [инструкция и глоссарий Индры](glossary-ru.md) — что
такое цепь, мост, выход, запасной канал и почему «готово» ≠ «всё открывается».
Офлайн-версия в тёмной теме — [glossary-ru.html](glossary-ru.html) (скачать и открыть
в браузере).

---

## 🙏 Спасибо / Thank you

<details>
<summary>По-русски</summary>

Tor сделали не мы. Мы им пользуемся, поэтому вот короткая выжимка: что это, кто это
сделал и за что этих людей стоит благодарить.

Onion routing придумали в середине 1990-х в Лаборатории военно-морских сил США:
математик **Пол Сайверсон** и его коллеги. Сеть Tor как программа вышла 20 сентября
2002 года, а **Роджер Динглдин** и **Ник Мэтьюсон** довели идею до работающей сети и
основали Tor Project — организацию, которая держит её до сих пор (на момент этой
записи стабильная версия — 0.4.9.14, от 7 октября 2026).

Смысл сети дорогой и простой: трафик идёт через несколько чужих компьютеров, и ни
один из них не видит одновременно, откуда он пришёл и куда уходит. Поэтому Tor
защищает от наблюдения и анализа трафика — и поэтому же его так упорно ломают.

Спасибо тем, кто искал в этой схеме ошибки: **Стивен Мёрдок**, **Иан Голдберг**,
**Кармела Тронкосо**, **Джейкоб Аппельбаум**. Атака на Tor — не предательство сети,
а часть её жизни: Tor Project сам называет атаки областью активных исследований и
приветствует их. Каждая опубликованная атака — либо дыра, которую закрыли, либо
граница, о которой теперь знают все. Работа эта неблагодарная: находишь слабое место
в том, что защищает людей, и портишь кому-то спокойную уверенность.

Спасибо тем, кто придумывает, как обойти блокировку. **Snowflake** — это сеть
прокси-мостов: волонтёры в странах, где Tor не заблокирован, отдают свой браузер как
временный мост, а человек под цензурой через него попадает в Tor. Автор — **Serene**,
работает с 24 января 2017 года, написан на Go и JavaScript, входит в Tor Browser и
Orbot. Здесь же — **Дэвид Файфилд**, **Сесилия Бокович**, **Филип Винтер**. Цензура
приходит первой, обход её — всегда догоняющая работа.

Спасибо тем, кто переписывает сеть на Rust, чтобы у неё было будущее, а не только
прошлое: **Иан Джексон**, **Александр Ферёй**. Проект называется Arti: полная замена
двадцатилетнего кода на C, начата в 2020-м, публично объявлена в июле 2021-го. Это не
смена языка ради моды — это попытка сделать так, чтобы ошибки в памяти перестали быть
способом деанонимизировать человека.

Спасибо тем, кто пишет сам Tor и считает его метрики: **Джордж Кадианакис**,
**Дэвид Гуле**, **Карстен Лёзинг**, **Тим Уилсон-Браун**, **Андреа Шепард**,
**Себастьян Хан**, **Изабела Багерос**. Спасибо тем, кто делает Tor Browser похожим на
обычный браузер, — чтобы человеку не нужно было выглядеть подозрительно, чтобы быть
свободным: **Георг Коппен**, **Ричард Поспесел**. Спасибо тем, кто занимается
криптографией, в которой мы не разбираемся: **Челси Комло**, **Исис Лавкруфт**.
И тем, кто спорит с сетью числами, а не мнениями: **Аарон Джонсон**, **Роб Джансен**.

Отдельно — тем, чьих имён не будет ни в одном списке авторов: кто держит relay на
своём сервере и платит за него сам; кто оставляет прокси Snowflake открытым в фоновой
вкладке; кто переводит интерфейс на язык, которого нет в списках; кто присылает
баг-репорт вместо того, чтобы молча уйти. Сеть без них не работает, а благодарят
обычно не их.

Мы пользуемся этим молча и каждый день, и ничего из этого не стоит нам ни копейки.
Поэтому говорим вслух: спасибо.

Мы не связаны с Tor Project и не говорим от его имени: это наша благодарность, а не
их одобрение.

</details>

<details>
<summary>In English</summary>

We did not build Tor. We use it, so here is the short version: what it is, who made
it, and why these people deserve thanks.

Onion routing was invented in the mid-1990s at the US Naval Research Laboratory by
mathematician **Paul Syverson** and his colleagues. Tor shipped as software on
20 September 2002, and **Roger Dingledine** and **Nick Mathewson** turned the idea into
a working network and founded the Tor Project, which still runs it (at the time of
writing the stable release is 0.4.9.14, dated 7 October 2026).

The design is expensive and simple: traffic passes through several machines, and none
of them sees both where it came from and where it goes. That is what protects users
from surveillance and traffic analysis — and that is why people keep trying to break it.

Thanks to those who looked for flaws in that design: **Steven Murdoch**, **Ian Goldberg**,
**Carmela Troncoso**, **Jacob Appelbaum**. An attack on Tor is not a betrayal of the
network but part of its life: the Tor Project calls attacks an active area of research
and welcomes them. Every published attack is either a hole that got closed or a limit
that everyone now knows about. The work is thankless: you find the weak spot in
something that protects people, and you take away somebody's peace of mind.

Thanks to those who invent ways around blocking. **Snowflake** is a network of proxy
bridges: volunteers in countries where Tor is not blocked lend their browser as a
temporary bridge, and a person under censorship reaches Tor through it. Its original
author is **Serene**; it has been around since 24 January 2017, written in Go and
JavaScript, and ships with Tor Browser and Orbot. **David Fifield**, **Cecylia Bocovich**
and **Philipp Winter** work in the same field. Censorship always arrives first;
circumvention is always the catch-up work.

Thanks to those rewriting the network in Rust, so it has a future and not only a past:
**Ian Jackson**, **Alexander Færøy**. The project is called Arti — a full replacement
for twenty-year-old C code, started in 2020 and announced publicly in July 2021. It is
not a language change for fashion: it is an attempt to stop memory bugs from being a
way to unmask a person.

Thanks to those who write Tor itself and measure its health: **George Kadianakis**,
**David Goulet**, **Karsten Loesing**, **Tim Wilson-Brown**, **Andrea Shepard**,
**Sebastian Hahn**, **Isabela Bagueros**. Thanks to those making Tor Browser look like
an ordinary browser, so a person does not have to look suspicious to be free:
**Georg Koppen**, **Richard Pospesel**. Thanks to those doing the cryptography we do not
understand: **Chelsea Komlo**, **Isis Lovecruft**. And to those arguing with the network
in numbers rather than opinions: **Aaron Johnson**, **Rob Jansen**.

And to everyone who will never appear in a credits file: the one running a relay on
their own server and paying for it; the one leaving a Snowflake proxy open in a
background tab; the one translating an interface into a language nobody lists; the one
filing a bug report instead of quietly walking away. The network does not work without
them, and they are usually the last to be thanked.

We use all of this silently, every day, and none of it costs us a penny. So we say it
out loud: thank you.

We are not affiliated with the Tor Project and do not speak for it: this is our
gratitude, not their endorsement.

</details>

---

Контакты: [Telegram](https://t.me/lightclove)
