# ⏱ React Auto Counter

## 🎯 Kaj se učim
- useEffect z intervalom
- cleanup funkcija
- dependency array
- functional state update
- start / stop logika

## 🧠 Ključni koncept

Interval ustvarimo samo, ko je `isRunning = true`.

Ko se `isRunning` spremeni:
1. React najprej pokliče cleanup
2. Nato ustvari nov interval (če je potrebno)

To prepreči memory leak.

## 🔥 Zakaj uporabljamo:
setCount(prev => prev + 1)

Da se vedno uporabi najnovejša vrednost state-a.

https://codesandbox.io/p/sandbox/hhmh7s?file=%2Fsrc%2FApp.js
