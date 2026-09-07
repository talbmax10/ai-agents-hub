# 🤖 AI Agents Hub — مركز وكلاء الذكاء الاصطناعي

<p align="center"><strong>دليل منظم لوكلاء الذكاء الاصطناعي والأدوات والمهارات وخوادم MCP وواجهات API للنماذج.</strong><br><sub>أُنشئ لمحبي وكلاء الذكاء الاصطناعي — اكتشف، قارن، ثبّت، طوّر، وابنِ.</sub></p>

<p align="center"><a href="README.md"><strong>🇬🇧 English</strong></a> · <a href="README.ar.md"><strong>🇸🇦 العربية</strong></a> · <a href="docs/index.html"><strong>🌐 واجهة المركز</strong></a></p>

> **أُنشئ AI Agents Hub لمحبي وكلاء الذكاء الاصطناعي.** وهو دليل وقاعدة معرفة تجمع الوكلاء وقدراتهم وMCP ومزودي النماذج.

## ✨ ماذا ستجد هنا؟

- 🔎 اكتشاف الوكلاء حسب النوع والاستخدام.
- 🏆 ترتيب تحريري قابل للمراجعة، وليس Benchmark رسميًا.
- 📦 أدلة تنصيب عملية.
- 🔗 روابط إلى المستودعات الأصلية.
- 🧩 أدوات ومهارات وMCP وتكاملات.
- 🆓 دليل مزودي API المجانيين أو ذوي الخطط المجانية.
- 🌍 توثيق عربي وإنجليزي متطابق في النطاق والمحتوى الأساسي.

## 🏆 الوكلاء المميزون

| الترتيب | الوكيل | النوع | مناسب لـ | التقييم |
|---:|---|---|---|---:|
| 1 | [Hermes Agent](https://github.com/NousResearch/hermes-agent) | شخصي/برمجة/ذاتي | سير العمل المستمر | ⭐ 9.7 |
| 2 | [OpenHands](https://github.com/All-Hands-AI/OpenHands) | برمجة/ذاتي | هندسة البرمجيات | ⭐ 9.6 |
| 3 | [OpenCode](https://github.com/anomalyco/opencode) | طرفية/برمجة | التطوير المرن مع المزودين | ⭐ 9.5 |
| 4 | [Cline](https://github.com/cline/cline) | IDE/برمجة | البرمجة بمشاركة الإنسان | ⭐ 9.4 |
| 5 | [Goose](https://github.com/block/goose) | عام/برمجة | سير عمل MCP | ⭐ 9.3 |
| 6 | [Aider](https://github.com/Aider-AI/aider) | طرفية/برمجة | Git والبرمجة التعاونية | ⭐ 9.2 |
| 7 | [SWE-agent](https://github.com/SWE-agent/SWE-agent) | بحث/برمجة | مهام GitHub وSWE | ⭐ 9.0 |
| 8 | [Gemini CLI](https://github.com/google-gemini/gemini-cli) | طرفية/برمجة | سير عمل Gemini | ⭐ 8.9 |
| 9 | [Qwen Code](https://github.com/QwenLM/qwen-code) | طرفية/برمجة | النماذج المفتوحة | ⭐ 8.8 |
| 10 | [OpenClaw](https://github.com/openclaw/openclaw) | شخصي/أتمتة | المراسلة والأتمتة | ⭐ 8.8 |

## 🧰 الأدوات والمهارات وMCP

تم توسيع المتجر ليشمل أتمتة المتصفح، البرمجة، البحث وRAG، الذاكرة وقواعد البيانات المتجهية، المراسلة، الأتمتة والتحكم بالحاسوب.

- 📚 [كتالوج الأدوات والمهارات الموسع](skills/catalog.ar.md)
- 🔌 [خوادم وتكاملات MCP](skills/mcp.md)
- 🧰 [واجهة المتجر](skills/README.md)

ومن الأدوات المدرجة: Playwright، Puppeteer، browser-use، GitHub CLI، Git، ripgrep، Docker، LlamaIndex، LangChain، Qdrant، Chroma، Redis، Telegram، Discord، n8n، PyAutoGUI وغيرها.

وتستخدم الإدخالات تصنيفات: Native، MCP، Plugin، Manual، Unverified. هذه التصنيفات للمساعدة في الاكتشاف وليست ضمانًا للتوافق.

## 🆓 مزودو API مجانيون أو بخطة مجانية

أضفنا دليلًا عمليًا لإنشاء مفتاح API، اختيار النموذج، إعداد الوكيل، والتعامل مع الحصص والأمان.

- 🆓 [دليل مزودي API المجانيين](providers/free-api.ar.md)

| المزود | نقطة البداية | متغير المفتاح |
|---|---|---|
| Google AI Studio / Gemini | أسهل بداية وتجارب Gemini | `GEMINI_API_KEY` |
| Groq | استدلال سريع | `GROQ_API_KEY` |
| OpenRouter | نماذج كثيرة عبر API واحد | `OPENROUTER_API_KEY` |
| Cerebras | استدلال سريع عندما يكون مؤهلًا | `CEREBRAS_API_KEY` |
| Cloudflare Workers AI | تطبيقات Cloudflare | إعداد الحساب والـbinding |

قد تتغير مجانية النماذج والحصص والتوفر؛ لوحة المزود الحالية هي المرجع.

## 🔑 كيف تنشئ مفتاح API وتختار النموذج؟

1. أنشئ حسابًا لدى المزود.
2. افتح قسم API Keys أو Developer.
3. أنشئ المفتاح واحفظه بأمان.
4. ضعه في متغير بيئة أو مدير أسرار.
5. اختر نموذجًا متاحًا حاليًا من قائمة المزود.
6. اضبط الوكيل باستخدام تنسيق API وBase URL ومعرّف النموذج الرسميين.
7. اختبر Tool Calling وطول السياق قبل المهام المستقلة الطويلة.

مثال:

```bash
export OPENROUTER_API_KEY="YOUR_KEY"
```

**لا تضع مفتاح API حقيقيًا داخل GitHub.**

## 📚 التوثيق

- 📋 [كتالوج الوكلاء](agents/README.md)
- 🧰 [متجر الأدوات والمهارات](skills/README.md)
- 🔌 [منظومة MCP](skills/mcp.md)
- 🆓 [واجهات API المجانية](providers/free-api.ar.md)
- 📦 [أدلة التنصيب](docs/installation.md)
- 📊 [منهجية الترتيب](docs/ranking.md)
- 🏗️ [البنية](docs/architecture.md)
- 🤝 [دليل المساهمة](CONTRIBUTING.md)
- 🔐 [سياسة الأمان](SECURITY.md)

## 🌍 ثنائي اللغة

النسختان العربية والإنجليزية متطابقتان في النطاق والمحتوى الأساسي: الوكلاء، الأدوات والمهارات، MCP، مزودو API المجانيون، الإعداد، الأمان والمساهمة.

- 🇬🇧 English: `README.md`
- 🇸🇦 العربية: `README.ar.md`
- 🌐 الواجهة التفاعلية: `docs/index.html`

## 🔐 الأمان أولًا

قد ينفذ الوكيل أوامر ويعدل ملفات ويتصل بالشبكة ويتحكم بالحاسوب. استخدم أقل صلاحيات ممكنة ولا تضع مفاتيح API أو كلمات المرور أو مفاتيح SSH في Issues أو Pull Requests أو المصدر.

## 🤝 المساهمة

يمكنك إضافة وكلاء، أدوات، مهارات، MCP، أدلة مزودي النماذج، تقارير توافق، Benchmarks، ترجمات وتحسينات للتوثيق. راجع [`CONTRIBUTING.md`](CONTRIBUTING.md).

## 📜 الترخيص

توثيق هذا الدليل مرخص MIT. المشاريع الخارجية تحتفظ بتراخيصها وعلاماتها التجارية. AI Agents Hub دليل مجتمعي مستقل.
