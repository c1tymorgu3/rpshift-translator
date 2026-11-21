# RPShift Translator

![RPShift Logo](logo.png)

**[English](#english) | [Türkçe](#türkçe)**

---

<a id="english"></a>
## English

### What it is

A translator for roleplay servers. Paste Turkish, get English that reads like a
person on a GTA V RP server actually talks, not like a dictionary. DeepL handles
the meaning, Groq handles the slang.

### Modes

1. **Groq only.** Fast, loose.
2. **Groq slang.** Translates and slangifies in one pass. This is the one to use.
3. **DeepL only.** Exact, professional, no flavour.
4. **DeepL + Groq slang.** DeepL for meaning, Groq for style.

The tracking window shows the original text, the raw translation and the final
result side by side. A trigger key sends it; the result is typed into whatever
window you came from. Prefix your text with `/` and slangification is skipped, so
commands like `/me walks` stay intact.

### Install

**1. AutoHotkey v2**

The script needs AutoHotkey v2.0 or newer. Install it from
[autohotkey.com](https://www.autohotkey.com/) and pick "Install v2.0".

**2. API keys**

Both services have a free tier, and you need your own keys.

Groq: go to [console.groq.com](https://console.groq.com/keys), sign in, create a
key, copy it. It starts with `gsk_`.

DeepL: go to [deepl.com/pro-api](https://www.deepl.com/pro-api), sign up for DeepL
API Free, then copy the authentication key from your account summary.

**3. Project setup**

Clone the repo, then create a file named `.env` next to the script:

```ini
DEEPL_API_KEY=your_deepl_key_here
GROQ_API_KEY=your_groq_key_here
```

**4. Run**

Double-click `groq.ahk`. The menu appears in the system tray.

### Using it

Select Turkish text anywhere, press `PageDown` (default, rebindable from the debug
menu), and the translation lands where you typed.

DeepL's free tier allows 500,000 characters a month. Groq's limit is per minute,
so long sessions are fine as long as you are not spamming.

---

<a id="türkçe"></a>
## Türkçe

### Nedir

Roleplay sunucuları için çevirmen. Türkçe yazdığını İngilizceye çevirir, ama
sözlük çevirisi gibi değil: GTA V RP sunucusunda konuşan birinin ağzıyla. Anlamı
DeepL, üslubu Groq yapar.

### Modlar

1. **Sadece Groq.** Hızlı, serbest.
2. **Groq slang.** Çevirir ve argoya çevirir, tek geçişte. Önerilen.
3. **Sadece DeepL.** Birebir, düzgün, süssüz.
4. **DeepL + Groq slang.** Anlam DeepL'den, üslup Groq'tan.

Takip penceresinde orijinal metin, ham çeviri ve son hâli yan yana durur. Tetik
tuşuyla çeviri gittiğin pencereye yazılır. Metnin başına `/` koyarsan argo
uygulanmaz, `/me walks` gibi komutlar bozulmaz.

### Kurulum

**1. AutoHotkey v2.** Script v2.0 ve üstünü ister.
[autohotkey.com](https://www.autohotkey.com/) üzerinden kur, "Install v2.0" seç.

**2. API anahtarları.** İkisinin de ücretsiz kotası var, anahtarları kendin alman
gerekir.

Groq: [console.groq.com](https://console.groq.com/keys), giriş yap, anahtar
oluştur, kopyala (`gsk_` ile başlar).

DeepL: [deepl.com/pro-api](https://www.deepl.com/pro-api), DeepL API Free'ye kaydol,
hesap özetinden authentication key'i al.

**3. Proje.** Repoyu indir, script'in yanına `.env` dosyası aç:

```ini
DEEPL_API_KEY=your_deepl_key_here
GROQ_API_KEY=your_groq_key_here
```

**4. Çalıştır.** `groq.ahk` dosyasına çift tıkla. Menü sistem tepsisinde çıkar.

### Kullanım

Herhangi bir yerde Türkçe metni seç, `PageDown` bas (varsayılan, debug menüsünden
değiştirilebilir), çeviri yazdığın yere düşer.
