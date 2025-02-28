---
title: Yii2
weight: 6
---

Inside a Yii2 application, you can use all methods from [the framework agnostic version](/docs/ray/v1/usage/framework-agnostic-php-project).

Additionally, you can use these Laravel specific methods.

### Showing events

You can display all events that are executed by calling `showEvents` (or `events`).

```php
ray()->showEvents();

Yii::$app->trigger('test-event', new TestEvent());

```

![screenshot](/docs/ray/v1/images/event.jpg)

To stop showing events, call `stopShowingEvents`.

```php
ray()->showEvents();

Yii::$app->trigger('myEvent', new MyEvent()); // this event will be displayed

ray()->stopShowingEvents();

Yii::$app->trigger('myEvent', new MyOtherEvent()); // this event won't be displayed.
```

Alternatively, you can pass a callable to `showEvents`. Only the events fired inside that callable will be displayed in Ray.

```php
Yii::$app->trigger('myEvent', new MyEvent()); // this event won't be displayed.

ray()->showEvents(function() {
    Yii::$app->trigger('myEvent', new MyEvent()); // this event will be displayed.
});

Yii::$app->trigger('myEvent', new MyEvent()); // this event won't be displayed.
```

### Enabling / disabling Ray

You can enable and disable sending stuff to Ray with the `enable` and `disable` functions.

```php
ray('one') // will be displayed in ray

ray()->disable();

ray('two') // won't be displayed in ray

ray()->enable();

ray('three') // will be displayed in ray
```

You can check if Ray is enabled or disabled with the `enabled` and `disabled` functions.

```php
ray()->disable();

ray()->enabled(); // false
ray()->disabled(); // true

ray()->enable();

ray()->enabled(); // true
ray()->disabled(); // false
```
