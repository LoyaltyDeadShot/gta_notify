# gta_notify
 A simple notification sistem for FiveM

This is a redesign and inspiration [mythic_notify](https://github.com/JayMontana36/mythic_notify)
Original Author: [@JayMontana36](https://github.com/JayMontana36)

# preview 👀

![](https://cdn.discordapp.com/attachments/1057014722274271343/1177819260777668619/image.png?ex=65f517aa&is=65e2a2aa&hm=2ac1856926d1d65ba1eb4aa33e25c479b4f098c5a8d6b4a3c407802edd5b86de&)

# usage

client.lua
```html
exports['gta_notify']:NormalNoti('notify', 'message')
```

server.lua
```html
TriggerClientEvent('gta_notify:client:SendAlert', source, { type = 'notify', text = 'texto' })
```

---

## Notify duration exports

- NormalNoti -> A normal notify duration
- LongNoti   -> A large notify duration
- CustomNoti -> Custom notify duration
- NotiFija   -> Infinite notify duration (You can end the notify :))

---

## NotiFija Usage

NotiFija Notifications Actions -
```html
exports['gta_notify']:NotiFija('start', 'notifijaidtest', 'success', 'NotiFija test. (Persist Noti)')
```

```html
exports['gta_notify']:NotiFija('end', 'notifijaidtest')
```

start (start the notification)
end (end the notification)


> NOTE: If you have a issue pls contact me on discord.

---

## Badges

- `badge-core`  -> A background for put yor server name
- `title`       -> A title class
- `icon`        -> a class for the icons of [Font Awesome](https://fontawesome.com)
- `bold`        -> a bold text class
- `<hr>`        -> it's a html code. It's a separation line

You need to put in <div class=""> the badge you are going to use

example:
```html
exports['gta_notify']:NormalNoti('notify', '<span class="title">Salary Notification</span>" .. xPlayer.Salary .. "<hr> <div class="badge-core">ROLEPLAYSERVER</div>')
```

---

This is a redesign and inspiration [mythic_notify](https://github.com/JayMontana36/mythic_notify)
Original Author: [@JayMontana36](https://github.com/JayMontana36)
