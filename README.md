# Home Assistant clock card
This is a simple clock card made for the Home Assistant Lovelace UI.

## 
![](https://i.imgur.com/L8CFpm6.gif "1")

The clock card requires the clock-card.js to be placed in the local (/www) folder on your Home Assistant installation and the following has to be put into the ui-lovelace.yaml file.
```
resources:
  - url: /local/clock-card.js
    type: js
```

The clock card can then be used by adding a 'manual-card' when configuring the UI.
```
...
  type: 'custom: clock-card'
  locale: <iso language code>
  style: 'both' | 'time' | 'date'
  timeStyle: 'full' | 'long' | 'medium' | 'short'
  dateStyle: 'full' | 'long' | 'medium' | 'short'

```

'en-US' is default as locale.</br>
'both' is default as style.</br>
'medium' is default, both for time and date format


