# Expert Systems (ES)
### Knowledge Base · CS 2nd Material

---

## What is an Expert System?

**ES** is a branch of **Artificial Intelligence** concerned with the concepts and methods of **symbolic inference** (reasoning) by a computer — and how the knowledge used to make those inferences is represented inside the machine.

> تخيل إن عندك دكتور في جيبك — مش دكتور حقيقي، لكن كمبيوتر عارف كل اللي الدكتور ده شايله في دماغه، وبيقدر يجاوبك وينصحك في أي وقت من غير ما تحتاج حد.

ال ES ده بيعمل **3 حاجات أساسية:**
- يحاكي قرارات الخبير البشري في مجال معين
- يجاوب على أسئلة ويوضح uncertainties
- يشتغل 24/7 من غير ما يتعب أو ينسى

---

## How It Works — إزاي بيشتغل؟

الـ ES قايم على **جزئين رئيسيين:**

**1. Knowledge Base (KB)**
المكان اللي بيخزن فيه كل المعلومات والقواعد اللي الخبير يعرفها — زي عقل الخبير بالظبط، بس داخل الكمبيوتر.

**2. Inference Engine**
ده "عقل" النظام اللي بياخد المعلومات من الـ KB ويشتغل عليها عشان يوصل للحل — بيشتغل بطريقتين:
- **Forward Chaining** → يبدأ من البيانات المتاحة ويوصل للنتيجة
- **Backward Chaining** → يبدأ من النتيجة ويرجع يشوف محتاج إيه

---

## Human Expert vs. Expert System

| Feature | Human Expert | Expert System |
|---|---|---|
| Time Availability | Workday فقط | **Always** |
| Geographic | Local | **Anywhere** |
| Safety | Irreplaceable | Replaceable |
| Consumable | Yes | **No** |
| Performance | Variable | **Consistent** |
| Speed | Variable | **Consistent (usually faster)** |
| Cost | High | **Reasonable** |

---

## History — شوية تاريخ

- الـ ES اتعرف على إيد **Edward Feigenbaum** في جامعة Stanford — وده اللي بيُعرف بـ *"أبو الـ Expert Systems"*
- في نفس الوقت تقريباً، **John McCarthy** في MIT اخترع لغة **LISP** — اللي بقت اللغة الرئيسية لبرمجة الـ AI والـ ES
- في الـ **1960s و 1970s** بدأ الـ ES يتطبق في الصناعة: **DENDRAL, MYCIN, XCON**
- آخر الـ **1980s** — أكتر من نص شركات الـ Fortune 500 كانت بتطور أو بتصون Expert Systems

---

## When Is an ES Needed? — امتى بنحتاجه؟

الـ ES بيفيد لما:

- الـ experts **مش متاحين دايمًا** — الـ ES يشتغل في أي وقت وأي مكان
- الخبراء البشريين **مش 100% reliable** أو consistent
- الخبير **مش كويس في شرح** قراراته
- المجال **نادر ومحتاج توزيع** واسع للمعرفة
- المواقف **خطيرة** زي الفضاء أو البيئات الحرجة
- محتاج **second opinion** في قرارات مهمة
- المهمة فيها **reasoning ومعرفة** — مش حدس أو reflexes

---

## Advantages — المميزات

```
✔ Rapid prototype development
✔ Easier verification & maintenance
✔ Fast response + explains its reasoning
✔ Cost effective
✔ Automated consistency checking in the KB
```

وفيه مميزات تانية مهمة أوي:

- **Permanence** — الـ ES مبينساش، لكن الخبير البشري ممكن ينسى
- **Reproducibility** — تقدر تعمل منه نسخ كتير، بدل ما تدرّب خبراء جدد بتكلفة عالية
- **Efficiency** — بيزود الـ throughput ويقلل التكلفة. غالي تبنيه، لكن **رخيص تشغّله**
- **Documentation** — بيوفر توثيق دائم لكل قرار
- **Completeness** — بيراجع كل الـ transactions، الخبير البشري بيراجع عينة بس
- **Consistency** — مش بيتأثر بـ recency effects زي البشر

---

## Disadvantages — العيوب

```
✘ صعب تبنيه — خصوصاً مرحلة جمع الخبرة
✘ مقدرش يرجع لمعرفة عامة لما يتعالق
✘ معندوش معرفة كافية عن نفسه وعن حدوده
✘ Knowledge Acquisition bottleneck
✘ ممكن يغلط لو الـ KB فيها معلومات غلط
```

وكمان:
- **No Common Sense** — معندوش حس سليم
- **No Creativity** — الخبير البشري بيتعامل مع المواقف الغريبة بإبداع، الـ ES ما يعرفش
- **No Self-Learning** — مش بيتحدث نفسه، لازم حد يحدثه manually
- **Degradation** — مش بيعرف يقول "المشكلة دي خارج تخصصي"

---

## ES Components — المكونات

### Inference Engine
عقل النظام — بياخد المعلومات ويطبق عليها القواعد ويقرر إيه الأسئلة اللي يسألها للمستخدم وبأي ترتيب.

يشتغل بطريقتين:
- **Forward Chaining** — من البيانات للنتيجة
- **Backward Chaining** — من النتيجة للبيانات المطلوبة

### Knowledge Base (KB)
بيخزن كل الحقائق والقواعد عن المجال — وبيوصلها للـ Inference Engine بشكل يقدر يستخدمه.

### User Interface
الواجهة اللي بتربط المستخدم بالنظام — بتاخد أسئلته وتترجمها لتعليمات يفهمها النظام.

### Working Memory
بتخزن المعلومات الخاصة بالمشكلة الحالية اللي النظام شغال عليها دلوقتي.
```
Example: loves(Hala, eggs)
```

### Explanation & Justification
- **Explanation** — بيوريك خطوة بخطوة إزاي النظام وصل للنتيجة (tracing back the rules)
- **Justification** — بيقولك **ليه** النتيجة دي صح أو غالبًا صح

---

## Conventional vs. Expert Systems

| Conventional Systems | Expert Systems |
|---|---|
| المعلومات والمعالجة في برنامج واحد | الـ KB منفصلة عن الـ Inference Engine |
| البرنامج مبيغلطش | ممكن يغلط |
| محتاج كل الـ input data | مش لازم كل البيانات |
| التعديل صعب | التعديل سهل — خصوصاً في الـ rules |
| بيشتغل لو اكتمل بس | يقدر يشتغل بجزء من الـ KB |
| الهدف الرئيسي: Efficiency | الهدف الرئيسي: Effectiveness |
| Numerical representation | Symbolic representation |

---

## Types of Expert Systems — الأنواع

**1. Rule-Based ES**
الأكتر شيوعاً — بيشتغل بقواعد IF-THEN اللي بيكتبها الخبراء البشر.
```
IF condition THEN action
```

**2. Fuzzy Logic ES**
بيتعامل مع البيانات الغامضة أو غير الدقيقة — مش بس صح/غلط، ممكن يقول "حار شوية" أو "حار جداً".
بيستخدم في product recommendations وimage recognition.

**3. Knowledge-Based ES**
عنده KB فيها حقائق وقواعد عن مجال محدد — بيقلد طريقة تفكير الخبير البشري في حل المشاكل.

**4. Neural Networks ES**
بيتعلم من البيانات — زي المخ البشري بالظبط، فيه خلايا عصبية صناعية بتربط بعضها وبتتعدل على حسب البيانات.
بيستخدم في: speech recognition، image classification، NLP.

---

## Applications — التطبيقات

| Application | Description | Examples |
|---|---|---|
| **Classification** | تصنيف object بناءً على خصائصه | — |
| **Diagnosis** | تشخيص عطل أو مرض من البيانات | CADUCEUS, MYCIN, PUFF |
| **Monitoring** | مقارنة بيانات نظام مستمر | REACTOR |
| **Design** | تصميم نظام على حسب المواصفات | DENDRAL, Dec Vax |
| **Scheduling & Planning** | تطوير أو تعديل خطة عمل | Mission Planning for AUV |
| **Interpretation** | استنتاج وصف الموقف من sensor data | PROSPECTOR |
| **Prediction** | توقع نتائج مواقف معينة | — |
| **Debugging** | حلول تدريجية لمشاكل معقدة | SAINT, MACSYMA |
| **Repair** | تنفيذ خطة علاج | Toxic Spill Crisis Management |
| **Control** | مراقبة وإصلاح سلوك الأنظمة | Space Shuttle Mission Control |

---

## Development Process — خطوات التطوير

```
1. Analyze System Requirements
   → افهم احتياجات المستخدم والمشكلة كويس

2. General Problem Definition
   → اعمل تعريف أعمق للمشكلة مع الخبير البشري

3. Knowledge Engineering
   → اجمع المعرفة، مثّلها، اتحقق منها

4. Prototype Development
   → اعمل نسخة أولية واختبر بيها

5. Verification & Validation
   → تأكد إن النظام ثابت ومتناسق ومقارنش بمستوى خبير حقيقي
```

---

## Development Tools — أدوات التطوير

| Category | Tools |
|---|---|
| Algorithmic Languages | C, Pascal, Visual Basic |
| Symbolic Languages | Prolog, LISP |
| Development Environments | Art, KEE, LOOPS |
| Expert System Shells | JESS, CLIPS |

**إزاي تختار الأداة الصح؟**

- نوع المعرفة وطريقة تفكير الـ ES
- الوقت والميزانية المتاحة
- خبرة الفريق في البرمجة
- الهاردوير المتاح للتطوير والتشغيل
- الأداء المطلوب من النظام

---

## Participants — مين بيشارك في التطوير؟

**Expert**
الشخص اللي عنده الخبرة الكبيرة في المجال — من غيره النظام مش هينجح. الأنظمة الكبيرة بتحتاج أكتر من خبير واحد.

**Knowledge Engineer**
زي المترجم — بياخد المعرفة من الخبير ويحولها لشكل يفهمه الكمبيوتر. لازم يعرف يختار الأدوات الصح.

**User**
اللي هيستخدم النظام في الآخر — رأيه مهم جداً، خصوصاً في الأنظمة الكبيرة.

---

## Future Prospects — المستقبل

- **Integration with AI & ML** — دمج الـ ES مع Machine Learning عشان يبقى أكتر تكيفاً مع البيانات المعقدة والـ real-time data
- **Personalized Decision Support** — الـ ES هيلعب دور أكبر في دعم القرارات الشخصية في الصحة والتعليم والمال
- **Cross-Domain Expertise** — الأنظمة المستقبلية ممكن تجمع بين مجالات مختلفة وتحل مشاكل متعددة الأبعاد
