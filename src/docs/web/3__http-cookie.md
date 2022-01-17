---
title: HTTP куки
date: "20-09-2020"
spoiler: Cookie - небольшой фрагмент данных, отправляемый сервером на браузер пользователя.
---

---

**HTTP cookie (web cookie, cookie браузера)** - это небольшой фрагмент данных, отправляемый сервером на браузер пользователя, который тот может сохранить и отсылать обратно с новым запросом к данному серверу. Это, в частности, позволяет узнать, с одного ли браузера пришли оба запроса (например, для _аутентификации пользователя_). Они запоминают информацию о состоянии для протокола HTTP, который сам по себе этого делать не умеет.

> Cookie используются, главным образом, для:
>
> - Управления сеансом (логины, корзины для виртуальных покупок)
> - Персонализации (пользовательские предпочтения)
> - Мониторинга (отслеживания поведения пользователя)

До недавнего времени cookie принято было использовать в качестве хранилища информации на стороне пользователя. Это могло иметь смысл в отсутствии вариантов, но теперь, когда в распоряжении браузеров появились различные **API** (программные интерфейсы приложения) для хранения данных, это уже не так.

Из-за того, что **cookie** пересылаются с каждым запросом, они могут слишком сильно снижать производительность (особенно в мобильных устройствах). В качестве хранилищ данных на стороне пользователя вместо них можно использовать **Web storage API** (_localStorage_ and _sessionStorage_) и **IndexedDB**.