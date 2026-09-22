# App Store Connect — metadata draft

Everything here is a draft to paste into App Store Connect. Limits: name 30, subtitle 30, promotional text 170, keywords 100 (comma-separated, no spaces), description 4000.
Brand name: **Pivotread** (chosen 2026-09-22 from the shortlist in `RELEASE_BACKLOG.md`, section 8 — checked free in the App Store US/RU, on the web and by DNS on 2026-09-21). Not yet reserved in App Store Connect; do that before the first submission, since the name is unique across the store.

## Fixed answers

| Field | Value |
|---|---|
| Primary category | Books |
| Secondary category | Productivity (or Education — try both) |
| Age rating | 4+ (no objectionable content, no web access, no user-generated content) |
| Price | Free (decide with the monetisation plan) |
| App Privacy | **Data Not Collected** (no analytics, no SDKs, no network requests) |
| Export compliance | No non-exempt encryption (`ITSAppUsesNonExemptEncryption = NO` is already set) |
| Sign-in required | No |
| Privacy Policy URL | host `docs/privacy-policy.md` (GitHub Pages) and paste the URL |
| Support URL | a page or repo issues URL with the contact e-mail `iosncik@yandex.ru` |

When analytics or another SDK is added later, the App Privacy answers and `PrivacyInfo.xcprivacy` must be updated in the same release.

## English (U.S.)

**Name:** `Pivotread: Speed Reader` (23)
**Subtitle:** `Read faster, word by word` (25)
**Keywords:** `speed reading,rsvp,reader,epub,pdf,fb2,focus,read faster,books,wpm,spritz,speedreader,text` (90)
**Promotional text (170):**
Read PDFs, EPUBs and articles at your own pace — one word at a time, eyes still, focus on. No account, no ads, works offline.

**Description:**

Read faster without losing the thread.

The app shows one word at a time, with the key letter always in the same spot, so your eyes never have to jump across the line. Pick a comfortable speed, tap play and let the words come to you.

READ WHAT YOU ALREADY HAVE
• PDF, EPUB, FB2, DOCX, TXT, RTF, HTML and Markdown
• "Open in…" from Files, Mail, Telegram or Safari
• Everything stays on your device — no account, no sign-in, no ads

A READER THAT GETS OUT OF THE WAY
• Tap to pause, tap again to continue
• Press and hold to see the text around the word, tap any word to continue from there
• Swipe to go back to the start of the sentence or jump to the next one
• Drag the progress bar to move through the book; see how much time is left
• Automatic pauses at commas, sentence ends and paragraphs — tunable to taste

MADE COMFORTABLE
• Four themes: OLED black, graphite, sepia and paper
• Choose your highlight colour (red, orange, blue, green, purple), typeface and text size
• Reading position is saved automatically; pick up exactly where you stopped
• Speeds from 60 to 1000 words per minute
• Screen stays awake while you read; playback pauses when you switch apps

Your books, your pace. Start with the built-in sample and find your speed.

**What's New (1.0):** First release.

## Русский

**Название:** `Pivotread: Скорочтение` (22)
**Подзаголовок:** `Читайте по одному слову` (23)
**Ключевые слова:** `скорочтение,быстрое чтение,читалка,rsvp,книги,epub,pdf,fb2,фокус,слов в минуту,чтение,текст` (91)
**Рекламный текст (170):**
Читайте PDF, EPUB и статьи в своём темпе: по одному слову, глаза неподвижны, внимание на тексте. Без аккаунта и рекламы, работает офлайн.

**Описание:**

Читайте быстрее, не теряя мысль.

Приложение показывает по одному слову, а главная буква всегда стоит на одном месте, поэтому глазам не нужно бегать по строке. Выберите удобную скорость, нажмите «play» и позвольте словам приходить к вам.

ЧИТАЙТЕ СВОИ ФАЙЛЫ
• PDF, EPUB, FB2, DOCX, TXT, RTF, HTML и Markdown
• «Открыть в…» из Файлов, Почты, Telegram и Safari
• Всё хранится на устройстве — без аккаунта, без входа, без рекламы

ЧИТАЛКА, КОТОРАЯ НЕ МЕШАЕТ
• Нажмите, чтобы поставить на паузу, и ещё раз — чтобы продолжить
• Задержите палец, чтобы увидеть текст вокруг слова, и нажмите любое слово, чтобы продолжить с него
• Свайпом вернитесь к началу предложения или перейдите к следующему
• Перетаскивайте полосу прогресса, чтобы перемещаться по книге; видно, сколько осталось
• Автоматические паузы на запятых, концах предложений и абзацах — настраиваются

УДОБНО ГЛАЗАМ
• Четыре темы: OLED-чёрная, графит, сепия и бумага
• Цвет акцента (красный, оранжевый, синий, зелёный, фиолетовый), шрифт и размер текста
• Позиция чтения сохраняется автоматически — продолжайте с того же места
• Скорость от 60 до 1000 слов в минуту
• Экран не гаснет во время чтения; при переключении на другое приложение чтение ставится на паузу

Ваши книги, ваш темп. Начните со встроенного примера и найдите свою скорость.

**Что нового (1.0):** Первый релиз.

## App Review notes

No account or sign-in is needed and the app makes no network requests.
Quick test: launch the app, go through the three onboarding screens and choose "Read the sample" — the built-in text starts playing. To try your own file: Library → "+" → pick a PDF, EPUB or TXT from Files. Tap the screen to pause; press and hold on the word to see the surrounding text.

## Screenshot plan (6.9″ and 6.5″, EN + RU)

1. Reader, dark theme, one big word with the red pivot letter — caption: "One word at a time" / «По одному слову».
2. Sepia theme with the serif font — "Themes and fonts that suit your eyes" / «Темы и шрифты под ваши глаза».
3. Context overlay with the current word highlighted — "Lost the thread? See the text around it" / «Потеряли мысль? Посмотрите текст вокруг».
4. Library with progress bars — "Every book remembers your place" / «Каждая книга помнит, где вы остановились».
5. Settings with the live preview — "Make it yours" / «Настройте под себя».
6. Finish card with words / time / average speed — "See how fast you read" / «Узнайте свой темп».

Debug builds can jump straight to a tab for capture: `xcrun simctl launch <device> <bundle-id> -openTab settings` (or `library`).

## Before the first submission

- [ ] Reserve "Pivotread" in App Store Connect.
- [ ] Host the privacy policy; fill in the Privacy Policy and Support URLs.
- [ ] Set `AppInfo.privacyPolicyURL` and `AppInfo.appStoreID` in `AboutViewController.swift` once they exist (the "Privacy Policy" and "Rate" rows stay hidden until then).
- [ ] Archive with the current Xcode SDK, upload to TestFlight, run the beta for a week.
- [ ] Capture screenshots in both languages.
