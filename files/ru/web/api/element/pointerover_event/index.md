---
title: "HTMLElement: pointerover event"
slug: Web/API/Element/pointerover_event
---

{{APIRef}}

Событие `pointerover` когда указатель входит в границы элемента обрабатываемого события.

<table class="properties">
  <tbody>
    <tr>
      <th scope="row">Bubbles</th>
      <td>Yes</td>
    </tr>
    <tr>
      <th scope="row">Cancelable</th>
      <td>Yes</td>
    </tr>
    <tr>
      <th scope="row">Interface</th>
      <td>{{domxref("PointerEvent")}}</td>
    </tr>
    <tr>
      <th scope="row">Event handler property</th>
      <td>
        <code
          ><a href="/ru/docs/Web/API/GlobalEventHandlers/onpointerover"
            >onpointerover</a
          ></code
        >
      </td>
    </tr>
  </tbody>
</table>

## Примеры

С использованием `addEventListener()`:

```js
const para = document.querySelector("p");

para.addEventListener("pointerover", (event) => {
  console.log("Pointer moved in");
});
```

С использованием свойство элемента `onpointerover` :

```js
const para = document.querySelector("p");

para.onpointerover = (event) => {
  console.log("Pointer moved in");
};
```

## Спецификации

{{Specifications}}

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- [`gotpointercapture`](/ru/docs/Web/API/Element/gotpointercapture_event)
- [`lostpointercapture`](/ru/docs/Web/API/Element/lostpointercapture_event)
- [`pointerenter`](/ru/docs/Web/API/Element/pointerenter_event)
- [`pointerdown`](/ru/docs/Web/API/Element/pointerdown_event)
- [`pointermove`](/ru/docs/Web/API/Element/pointermove_event)
- [`pointerup`](/ru/docs/Web/API/Element/pointerup_event)
- [`pointercancel`](/ru/docs/Web/API/Element/pointercancel_event)
- [`pointerout`](/ru/docs/Web/API/Element/pointerout_event)
- [`pointerleave`](/ru/docs/Web/API/Element/pointerleave_event)
- [`onpointerover`](/ru/docs/Web/API/Element/pointerover_event) свойство-обработчик события
- Событие на элементах `Document`: событие [`pointerover`](/ru/docs/Web/API/Element/pointerover_event)
