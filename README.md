# مخزون الطبعات · print-stock

**متابعة مخزون القطع المطبوعة لطابعات Bambu Lab** — كم عندك، كم طبعت، كم
يساوي مخزونك، وش لازم تطبع.

<div dir="rtl">

## التشغيل — ولا يحتاج جهازك تثبيت أي شيء

١. نزّل الـzip من [الإصدارات](https://github.com/relifeg1/print-stock-releases/releases) وافتحه في أي مجلد.
٢. شغّل **«مخزون الطبعات.bat»** — يفتح المتصفح على شاشة التهيئة.
٣. ثلاث خطوات، ويشتغل.

المشغّل (`node.exe`) **داخل المجلد**، فلا تحتاج تثبيت Node ولا أي برنامج.
ولاختصارٍ على سطح المكتب وتشغيلٍ مع الويندوز: افتح **«ثبّت الاختصارات.bat»** مرة واحدة.

## وين بياناتي؟

**على جهازك وحده.** تختار في شاشة التهيئة:

- **على جهازي** — الأسهل، بلا حساب ولا إنترنت. بياناتك في مجلد `data`.
- **في السحابة** — قاعدة مجانية على [neon.tech](https://neon.tech)، فتفتح مخزونك من الجوال ومن جهازٍ ثانٍ.

وتنقلها بينهما وقت ما تشاء من: **الإعدادات ← مكان بياناتك ← انقلها**.

> **لا خادمَ مشتركًا ولا حسابات.** كل نسخة مستقلّة ببياناتها. من ينزّل
> التطبيق يجد شاشة فارغة وبياناته وحده.

## وش يسوي

| | |
|---|---|
| **المخزون** | كم قطعة عندك من كل صنف، وأين هي على رفوفك |
| **الكتات** | قطعتان تُجمَّعان منتجًا — والتطبيق يعرف كم وحدة كاملة تقدر تجمّع |
| **الطابعات** | يقرأ طابعات Bambu مباشرةً: وش تطبع الآن، ومتى تفرغ |
| **تأكيد الطبعات** | الطابعة تقول اسم المهمة؛ أنت تقول أي صنف وكم خرج صالحًا |
| **خيوط الطباعة** | كم بقي من كل بكرة، ومتى تنفد بحسب استهلاكك |
| **الطابور** | ترتيب الطبعات القادمة بساعة الحائط — ولا يُرسل شيء إلا باعتمادك |
| **الأرقام** | قيمة مخزونك بالتكلفة، وما أنتجته، ونسب التلف |
| **الجوال** | نسخة مختصرة: سجّل · تابع · امسح باركود |

## النسخ الاحتياطي

يُكتب وحده عند كل تشغيل وكل ٢٤ ساعة في مجلد `backups`.
ونزّل نسخةً على مكانٍ ثانٍ من: **الإعدادات ← نزّل نسخة على جهازي** — والاستعادة من نفس الصفحة.

> **وبياناتك مسؤوليتك**: من يمسك مخزون رزقه ببرنامجٍ على جهازٍ واحد يجب أن
> يحفظ نسخةً في مكانٍ آخر.

## التحديث

**لا يتحدّث وحده أبدًا.** يفحص أسبوعيًّا، وإن نزل إصدار جديد يظهر لك في
الإعدادات مع «ما الجديد» — وأنت تقرّر: حدّث · لاحقًا · تجاهل هذه النسخة.
وقبل التركيب تُحفظ نسخةٌ احتياطية، والرجوع ضغطة.

## الوصول من خارج البيت

ضع رقمًا سريًّا من **الإعدادات ← القفل**، ثم افتح نفقًا
([Cloudflare Tunnel](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/)
أو [Tailscale](https://tailscale.com)). التطبيق يتعامل مع الأنفاق أصلًا.

> ⚠️ **ولا تفتحه للإنترنت بلا رقمٍ سري.** ومحاولات الدخول محدودة (خمسٌ في ربع
> ساعة) فلا يُكسر الرقم بالتخمين.

## الجوار — اختياري تمامًا

بُني بجانب تطبيقين على جهاز صاحبه: حاسبة تكلفة (Print-Costly) وسجل طبعات
(print-tracker). **ومن لا يملكهما لا ينقصه شيء**: التطبيق يفحص وجودهما
ويُخفي صفحاتهما بلا خطأ ولا رسالة غامضة.

## الرخصة

مجاني للاستخدام والنسخ والإهداء — انظر [LICENSE](LICENSE).
وشيفرة المصدر غير منشورة.

</div>

---

<div dir="ltr">

## English

**Inventory tracking for 3D-printed stock, built for Bambu Lab printers.**
How many parts you have, what you printed, what your stock is worth, what
needs printing.

### Running it

1. Download the zip from [Releases](https://github.com/relifeg1/print-stock-releases/releases) and extract anywhere.
2. Run **«مخزون الطبعات.bat»** — opens your browser on the setup screen.
3. Three steps and you're running.

`node.exe` ships **inside the folder** — nothing to install.

### Where your data lives

**On your own machine.** Pick at setup: local (no account, no internet —
stored in `data/`) or a free cloud database on [neon.tech](https://neon.tech)
so you can open it from your phone. Switch between them anytime from
Settings.

> **No shared server, no accounts.** Every copy is independent. Whoever
> downloads it starts empty, with only their own data.

### What it does

Stock levels per item and per shelf · kits assembled from parts (it knows
how many complete units you can build) · live Bambu printer status ·
per-print confirmation (the printer gives a job name; you say which item
and how many came out good) · filament spools with run-out forecasts · a
print queue ordered by wall clock, where **nothing is sent without your
approval** · stock value at production cost, output and scrap rates · and a
compact mobile view.

### Backups

Written automatically on every start and every 24h into `backups`. Download
a copy elsewhere from Settings — restoring is on the same page. **Keeping an
off-machine copy is your responsibility.**

### Updates

**Never automatic.** Checks weekly; if a release is out you get a note in
Settings with release notes, and you choose: update · later · skip this
version. A backup is taken before installing, and rollback is one click.

### Access from outside your home

Set a password in Settings → Lock, then run a tunnel (Cloudflare Tunnel or
Tailscale). The app already handles reverse proxies.

> ⚠️ **Never expose it without a password.** Login attempts are rate
> limited (5 per 15 minutes).

### Interface language

The interface is currently **Arabic only**. English is planned.

### Licence

Free to use, copy and share — see [LICENSE](LICENSE). Source code is not
published.

</div>
