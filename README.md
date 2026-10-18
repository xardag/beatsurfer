# ⚡ BeatSurfer Triki - Cyber Highway

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-00f0ff?style=for-the-badge&logo=github)](https://xardag.github.io/)
[![Organization](https://img.shields.io/badge/Organization-xardag-ff007f?style=for-the-badge&logo=github)](https://github.com/xardag)
[![Web Audio API](https://img.shields.io/badge/Web%20Audio-Procedural%20Synth-ffd700?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
[![Web Bluetooth](https://img.shields.io/badge/Web%20Bluetooth-Żabka%20Triki-00d672?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API)

> **BeatSurfer Triki** to dynamiczna, trójwymiarowa gra rytmiczna w klimacie synthwave i neonowego cyberpunku, wydana pod szyldem organizacji **[xardag](https://github.com/xardag)** na **GitHub Pages**. Gra jest w 100% samowystarczalna (jeden plik HTML, zero zewnętrznych bibliotek, synteza dźwięku proceduralnego w locie).

---

## 🎮 Zagraj online (GitHub Pages)

Gra dostępna jest bezpośrednio w przeglądarce pod adresem:
👉 **[https://xardag.github.io/](https://xardag.github.io/)**

Działa bez instalacji na **komputerach**, **tabletach** oraz **smartfonach**.

---

## ✨ Kluczowe Cechy

1. **Własny silnik syntezy i audio Web Audio API**:
   - Generuje w czasie rzeczywistym 3 dynamiczne utwory synthwave: *Cyber Drift (130 BPM)*, *Synth Overdrive (142 BPM)* i *Neon Pulse (124 BPM)*.
   - Możliwość wczytania dowolnego własnego pliku **MP3 / WAV / OGG**.
2. **Deterministyczny generator tras (100% powtarzalne High Score)**:
   - Każdy utwór analizowany jest algorytmem energii pasm (FFT) i generuje stały układ nut, pozwalając na uczciwą rywalizację o rekord trasy.
3. **Mnożniki Combo i Star Power**:
   - Ciągłe zbieranie nut podbija mnożnik (`x1` ➔ `x2` ➔ `x3` ➔ `x4`).
   - Gwiazdki ładują wskaźnik **Star Power**. Po naładowaniu powyżej 50% aktywacja podwaja mnożnik aż do **x8**!
4. **Tryb Pełnego Ekranu (Fullscreen)**:
   - Dedykowany przycisk `⛶ Pełny ekran` oraz skrót klawiszowy `F` dostosowują arenę do pełnych wymiarów ekranu na monitorach i telefonach.
5. **Pełna responsywność i sterowanie mobilne**:
   - Adaptacyjny układ dopasowany do ekranów dotykowych (zarówno w pionie, jak i w poziomie).
   - Wygodne przyciski dotykowe pod ekranem gry (`⬅️ LEWY`, `⏺️ ŚRODEK`, `PRAWY ➡️`, `⭐ STAR POWER`).
   - Bezpośrednie sterowanie dotykiem na płótnie (przesuwanie palcem, podwójne stuknięcie lub gest w górę aktywujący Star Power).
6. **Wsparcie dla kontrolera Żabka Triki (BLE)**:
   - Bezprzewodowa łączność przez Web Bluetooth API (Chrome / Edge / Opera / Android Chrome).
   - Dwa tryby sterowania:
     - **Biurko (Tabletop)**: kapsel leży na blacie, obrót jak kierownicą.
     - **W dłoni (Tilt)**: kapsel trzymany poziomo, wychylenie w lewo/prawo.
   - Fizyczny przycisk kapsla odpala Star Power, a dioda LED reaguje na stan rozgrywki.

---

## 🕹️ Sterowanie

### 💻 Komputer (Klawiatura / Mysz):
- **Skręt w lewo**: `A` lub `Strzałka w lewo`
- **Środek**: `S` / `W` lub `Strzałka w dół / w górę`
- **Skręt w prawo**: `D` lub `Strzałka w prawo`
- **Star Power**: `Spacja`, `E`, `Shift`
- **Pełny ekran**: `F` (lub przycisk w prawym górnym rogu)
- **Start / Restart**: `Spacja` lub kliknięcie przycisku
- **Mysz**: kliknięcie lub przeciąganie kursorem po trzech torach trasy

### 📱 Telefon / Tablet (Dotyk):
- **Przyciski ekranowe**: duże przyciski pod areną (`⬅️ LEWY`, `⏺️ ŚRODEK`, `PRAWY ➡️`, `⭐ STAR POWER`)
- **Dotyk na trasie**: dotknij wybranego pasa lub przeciągaj palcem
- **Gest Star Power**: podwójne stuknięcie w ekran lub szybki gest przesunięcia w górę (Swipe Up)
- **Pełny ekran**: kliknij `⛶ Pełny ekran` w pasku statusu

### 📡 Kontroler Żabka Triki (Bluetooth):
- **Połączenie**: kliknij `🔗 Połącz z Triki` w panelu bocznym
- **Sterowanie**: obracaj kapslem na blacie (tryb biurko) lub przechylaj w dłoni
- **Przycisk kapsla**: aktywacja Star Power / rozpoczęcie gry
- **Kalibracja**: przycisk `🎯 Kalibruj środek` pozwala wyzerować pozycję spoczynkową

---

## 🚀 Publikacja na GitHub Pages

Jeśli repozytorium to strona organizacji **[xardag.github.io](https://github.com/xardag/xardag.github.io)**:
1. Skopiowane pliki (`index.html`, `README.md`) w głównym katalogu repozytorium są natychmiast serwowane pod adresem:
   `https://xardag.github.io/`

Jeśli repozytorium to podprojekt np. **[beatsurfer](https://github.com/xardag/beatsurfer)**:
1. Przejdź do repozytorium w serwisie GitHub: **Settings** ➔ **Pages**.
2. W sekcji **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: `main` / `master`, folder: `/ (root)`
3. Kliknij **Save**. Strona będzie dostępna pod adresem:
   `https://xardag.github.io/beatsurfer/`

---

## 📄 Struktura plików

- `index.html` – główny punkt wejścia gry dla GitHub Pages (pełna, zoptymalizowana wersja)
- `beatsurfer_triki.html` – kopia kompatybilności bezpośredniej
- `README.md` – dokumentacja projektu i instrukcja obsługi

---

### © Organizacja [xardag](https://github.com/xardag)
Projekt przygotowany i zoptymalizowany dla organizacji GitHub **xardag**.
