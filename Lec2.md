# Knowledge Base & Knowledge Engineering
### Knowledge Base · CS 2nd Material

---

## Data, Information & Knowledge — الفرق بينهم

الناس كتير بتخلط بينهم، خليني أوضح:

**Data** — Raw unprocessed facts
> مجرد أرقام أو حقائق خام من غير معنى — static في طبيعتها، هي المادة الخام للمعلومات.
```
Example: 38.5 — مجرد رقم
```

**Information** — Meaning attached to data
> لما الداتا تتجمع وتتنظم وتتفسر — بتساعد في اتخاذ القرارات.
```
Example: 38.5°C → ده حرارة جسم المريض
```

**Knowledge** — Purpose and competence attached to information
> لما نفهم المعلومات ونعرف نعمل بيها حاجة — مشتقة من المعلومات زي ما المعلومات مشتقة من الداتا.
```
Example: حرارة 38.5°C → ده بيدل على infection → المريض محتاج علاج
```

---

## Two Views of the Hierarchy — نظرتين مختلفتين

**1. Hierarchical View (من تحت لفوق)**
```
Data → Information → Knowledge
```
المعلومات هي الخام الجديد للمعرفة — والمعرفة هي معلومة متحقق منها وشخصنة.

**2. Reversed Hierarchical View (من فوق لتحت)**
```
Knowledge → Information → Data
```
لازم يكون عندنا معرفة بالمجال الأول عشان نعرف نجمع إيه من داتا ونحوله لمعلومات.

---

## Knowledge Classification — أنواع المعرفة

| | Explicit Knowledge | Tacit Knowledge |
|---|---|---|
| **Definition** | know-what | know-how |
| **Nature** | Formalized & codified | لا تُعرَّف بكلمات أو أرقام |
| **Handling** | Easy to identify, store & retrieve | Very hard to handle |
| **Where** | Databases, memos, docs | Beliefs, intuition, mental models, technical skills |

> **Explicit** = المعلومات اللي تقدر تشرحها بسهولة وتكتبها
> **Tacit** = الخبرة الجوانية اللي اكتسبتها بالتجربة وصعب تشرحها بالكلام

---

## Knowledge Conversion — تحويل المعرفة

المعرفة الفعّالة بتتطلب **continuous conversion** بين النوعين — وعندنا 4 طرق:

**1. Externalization (Tacit → Explicit)**
الخبرة اللي في دماغ الشخص بتتحول لحاجة مكتوبة.
```
Example: طبيب بيكتب نتيجة تجربة سريرية كـ clinical practice recommendation
```

**2. Combination (Explicit → Explicit)**
معلومات مكتوبة بتتجمع مع بعض وتطلع معرفة جديدة.
```
Example: دمج medical knowledge مع organizational knowledge في decision support system
```

**3. Internalization (Explicit → Tacit)**
الشخص بيقرأ ويطبق حاجة مكتوبة لحد ما تبقى خبرة عنده.
```
Example: دكتور بيطبق CPG مرات كتير لحد ما يبقى جزء من خبرته الشخصية
```

**4. Socialization (Tacit → Tacit)**
خبرة بتنتقل لشخص تاني عن طريق المشاركة والتعلم المباشر.
```
Example: شاغل بيتعلم من المعلم، أو consensus بين خبراء في اجتماع طبي
```

```
         | to Tacit    | to Explicit
---------|-------------|-------------
from Tacit   | Socialization | Externalization
from Explicit | Internalization | Combination
```

---

## Knowledge Engineering

> هي **عملية استخراج وتنظيم وإضافة** المعرفة الجديدة لـ Knowledge Base، وتحسين المعرفة اللي اتجمعت قبل كده.

الهدف منها: توسيع قدرات النظام أو تحسين أداؤه في مهمة معينة.

المعرفة دي ممكن تكون على شكل:
```
facts · rules · concepts · procedures · heuristics
formulas · relationships · statistics
```

**بكل بساطة:** بنجيب النولدج من مصادرها (الخبير مثلاً)، نرتبها وننظمها، ونضيفها في الـ KB بتاعة الـ ES — وكمان نحسن النولدج القديمة لو محتاجة تعديل.

---

## Two Perspectives — نظرتين للـ Knowledge Engineering

**1. Narrow View (نظرة ضيقة)**
التعامل مع المعرفة نفسها جوه النظام:
- Knowledge Acquisition
- Knowledge Representation
- Inferencing
- Validation & Explanation
- Maintenance

**2. Broad View (نظرة واسعة)**
كل عملية بناء الـ intelligent systems من الأول للآخر:
- تصميم النظام
- إضافة المعرفة
- تشغيله وتطويره

> المعرفة عند الخبراء البشر غالباً غير منظمة وغير معبّر عنها بشكل صريح — وده اللي بيخلي الـ Knowledge Engineering صعبة.

---

## 3 Things Before Any ES Project

قبل ما تبدأ أي مشروع ES، لازم تجاوب على 3 أسئلة:

1. **هل المجال مناسب للـ ES أصلاً؟**
   → لازم تقيّم المجال وتتأكد إن نوع المعرفة فيه ينفع يتحول لـ ES

2. **مصدر الخبرة إيه؟**
   → لازم تحدد مصدر المعرفة وتتأكد إنه عنده المستوى المطلوب للمشروع

3. **لو المصدر بشر — إزاي هتطلع المعرفة منه؟**
   → لازم تحدد التقنيات والمشاركين في عملية الاستخراج

---

## Knowledge Engineering Process Activities — 3 نشاطات رئيسية

### 1. Knowledge Acquisition

> جمع المعرفة من الخبير أو المصادر المختلفة — تحليلها وتمثيلها بشكل يقدر النظام يستخدمه.

**التحديات اللي بتقابل العملية دي:**
- أغلب المعرفة في دماغ الخبراء مش مكتوبة
- الخبراء عندهم Tacit Knowledge صعب يشرحوها بالكلام
- الخبراء مشغولين ووقتهم غالي
- مفيش خبير واحد يعرف كل حاجة
- المعرفة ليها "shelf life" — بتتغير مع الوقت

**Knowledge Acquisition — 5 مراحل:**

```
1. Identification   → تحديد خصائص المشكلة
2. Conceptualization → إيجاد المفاهيم اللي هتمثل بيها المعرفة
3. Formalization    → تصميم هيكل لتنظيم المعرفة
4. Implementation   → كتابة الـ rules والـ frames فعلياً
5. Testing          → التحقق من صحة القواعد
```

**Knowledge Acquisition Methods — 3 طرق:**

**Manual**
الـ knowledge engineer بيكلم الـ expert مباشرة ويطلع منه المعرفة.
- Interviewing (structured / semi-structured / unstructured)
- Tracking the reasoning process
- Observing
> عيبها: بطيئة، مكلفة، وممكن تبقى غير دقيقة.

**Semi-Automatic**
بنستخدم أدوات وبرامج تساعد في جمع المعرفة — إما تساعد الخبير إنه يبني الـ KB بنفسه، أو تساعد الـ knowledge engineers يشتغلوا بشكل أسرع.

**Automatic (Machine Learning)**
النظام بيتعلم المعرفة من البيانات لوحده — دور الخبير والـ knowledge engineer بيقل أو بيختفي.
> لكن كلمة "Automatic" ممكن تكون مضللة — هيبقى دايماً فيه إنسان بيبني النظام ويشرف عليه.

---

**Difficulties in Knowledge Acquisition — الصعوبات:**

- الخبير ممكن ميعرفش يشرح معرفته أو ميقدرش
- الخبراء مشغولين أو مش عايزين يتعاونوا
- طرق الاستخراج ممكن تكون poorly defined
- المعرفة المطلوبة ممكن تكون موزعة على مصادر كتير
- صعب تميّز المعرفة المهمة وسط البيانات غير المرتبطة
- الخبير ممكن يغيّر سلوكه لما حد يراقبه أو يقابله
- مشاكل في التواصل بين الـ knowledge engineer والخبير

---

### 2. Knowledge Representation (KR)

> مجال في الـ AI هدفه تمثيل المعلومات بشكل يقدر الكمبيوتر يستخدمه لحل مشاكل معقدة — زي تشخيص مرض أو إجراء محادثة بلغة طبيعية.

الـ **Procedural Code** العادي مش مناسب لتمثيل المعرفة في الـ ES — الـ KR بيخلي البرامج المعقدة **أسهل في الفهم والتعريف والصيانة**.

---

## Knowledge Representation Methods

### 1. Logical Representations

لازم نحدد:
- **Syntax** — الرموز والقواعد اللي نقدر نكتب بيها جمل صحيحة
- **Semantics** — معنى الجمل دي وإزاي نقرأها صح

#### Propositional Logic
المعروفة بـ Sentential Logic أو Statement Logic.

- **Declarative** — بنقول حاجة صح أو غلط
- بتسمح بمعلومات جزئية / بدائل / منفية (مش زي قواعد البيانات العادية)
- **محدودة في التعبير** — مش يقدر يمثل كل أنواع المعرفة المعقدة

**الرموز:**
```
∧  → AND (conjunction)
∨  → OR (disjunction)
⇒  → IF...THEN (implication)
⟺  → IF AND ONLY IF (biconditional)
¬  → NOT (negation)
P, Q, S... → Propositional symbols (atomic sentences)
true, false → Logical constants
```

**Truth Table:**
```
P  | Q  | ¬Q | P∧Q | P∨Q | P→Q | P⟺Q
T  | T  | F  |  T  |  T  |  T  |  T
T  | F  | T  |  F  |  T  |  F  |  F
F  | T  | F  |  F  |  T  |  T  |  F
F  | F  | T  |  F  |  F  |  T  |  T
```

**مثال:**
```
P = "It is hot"
Q = "The sun is shining"
R = "Kids should wear hats"

P ∧ Q ⇒ R
```

**Well Formed Formula (WFF):**
- A symbol is a sentence
- If S is a sentence → ¬S is a sentence
- If S is a sentence → (S) is a sentence
- If S and T are sentences → (S∨T), (S∧T), (S⇒T), (S⟺T) are sentences

---

#### First-Order Logic (FOL)
المعروفة بـ First-order Predicate Calculus / Predicate Logic.

الفرق الأساسي عن Propositional Logic: بتستخدم **quantified variables**.

**Universal Quantifier (∀)** → "For all"
```
∀x man(x) → loves(x, soccer)
= "كل الرجال بيحبوا الكورة"
```

**Existential Quantifier (∃)** → "There exists"
```
∃x younger(x, Haneen)
= "فيه حد أصغر من حنين"
```

```
∀x P(X)                          ∃x P(X)
Universal Quantifier              Existential Quantifier

For All, every thing, every one   Some
P(x1) & P(x2) & ... & P(xn)     P(x1) ∨ P(x2) ∨ ... ∨ P(xn)
```

**Function Symbols** → map individuals to individuals
```
father-of(Mary) = John
color-of(Sky) = Blue
```

**Predicate Symbols** → map individuals to truth values
```
greater(5, 3)
green(Grass)
color(Grass, Green)
```

**Examples:**
```
Every gardener likes the sun.
∀x gardener(x) → likes(x, Sun)

All purple mushrooms are poisonous.
∀x (mushroom(x) ∧ purple(x)) → poisonous(x)

No purple mushroom is poisonous.
¬∃x purple(x) ∧ mushroom(x) ∧ poisonous(x)

There are exactly two purple mushrooms.
∃x ∃y mushroom(x) ∧ purple(x) ∧ mushroom(y) ∧ purple(y) ∧ ¬(x=y)

Clinton is not tall.
¬tall(Clinton)
```

---

### 2. Semantic Networks

> Graph structure بيمثل المعرفة في شكل **nodes وarcs** مترابطة.

- كل **node** = object أو concept
- كل **arc** = علاقة بين الـ nodes
- البشر طبيعياً بيخزنوا المعرفة في شكل graphs — وهي سهلة جداً تتخزن في البرامج

```
Person ──(is a)──> Adult Male ──(height)──> 178
                       │
                   (is a)
                       │
               Baseball Player ──(batting-avg)──> .282
```

---

### 3. Production Rule Representations (IF-THEN Rules)

> من أشهر طرق تمثيل المعرفة — بتستخدم قواعد IF-THEN.

**الأشكال المختلفة:**
```
IF condition THEN action (ADD / REMOVE / MODIFY)
IF premise THEN conclusion
IF p AND q are true THEN r is true
```

- الـ **IF part** = antecedent (left-hand side)
- الـ **THEN part** = consequent (right-hand side)

**المميزات:**
- **Modular** — كل rule مستقلة، تقدر تضيف/تمسح/تعدل من غير ما تأثر على الباقي
- مشهورة جداً في الـ ES

**العيب:**
- لو عدد الـ rules كبير — النظام بيبطأ

---

### 4. Frames Representations

> طريقة بنمثل بيها المعرفة عن حاجة معينة في شكل **ملف منظم**.

- المعلومات بتتخزن في **Slots** — كل slot فيها name وvalue
- الـ Frames ليها **hierarchical structure**

**نوعين من الـ Reasoning:**

**Matching** → يشوف الـ frame الأنسب للموقف الحالي
- صعب لأن الـ frames فيها تفاصيل كتير وmatchتام نادر

**Inheritance** → لو frame ناقص معلومة، بيجيبها من الـ parent
- بيتم باستخدام Depth-first أو Breadth-first

```
Hotel Room Frame:
  Superclass: room
  Location: hotel
  Contains: [hotel-chair, hotel-bed, hotel-phone, ...]
```

---

## Advantages & Disadvantages of KR Methods

| Scheme | Advantages | Disadvantages |
|---|---|---|
| **Production Rules** | Simple syntax, easy to understand, modular, flexible | Hard to follow hierarchies, inefficient for large systems, poor at descriptive knowledge |
| **Semantic Networks** | Easy hierarchy, easy to trace associations, flexible | Meaning might be ambiguous, exception handling is difficult |
| **Frames** | Expressive, easy to set up slots, easy to detect missing values | Difficult to program, lacks inexpensive software |
| **Formal Logic** | Facts asserted independently, only valid consequences, completeness | Inefficient with large data, very slow with large KBs |

---

### 3. Knowledge Validation & Verification (V&V)

> الطرق الوحيدة اللي بنقدر نحكم بيها على نجاح الـ KB development system — وبيوفروا طرق لقياس جودة المعرفة وتحديد أين يلزم تصحيح.

**Verification** — building the system right
> بنقول: هل السيستم اتبنى صح وطبّق المطلوب؟

- يمكن اعتباره جزء من الـ Validation
- مش كافي لوحده — لأن المتطلبات نفسها ممكن تكون غلط من الأول

**Validation** — building the right system
> بنقول: هل السيستم ده أصلاً بيعمل اللي المستخدم عايزه؟

```
Validation of Knowledge
├── Verification
│   └── Approaches based on:
│       decision tables · dependency charts
│       decision trees · graphs · machine learning
└── Evaluation
    └── Approaches aimed at:
        testing · generating · refinement
```

**KB Forms:** Procedural · Declarative · Mixed · Generated · Others

---

## Examples — أمثلة مهمة على الـ FOL

```
Every human, animal and bird is a living thing that breathes and eats.
∀X [[human(X) ∨ animal(X) ∨ bird(X)] ∧ eat(x) ∧ breath(x)] → living(X)

All birds are animals and can fly.
∀X bird(X) → animal(X) ∧ canfly(X)

Every man and woman who have two legs are humans.
∀X [[man(X) ∧ haslegs(X,2)] ∨ [woman(X) ∧ haslegs(X,2)]] → human(X)

Cat is an animal and has fur.
animal(cat) ∧ has(cat, fur)

All animals have skin and can move.
∀X animal(X) → has(X, skin) ∧ canmove(X)

Giraffe is an animal who is tall and has long legs.
animal(giraffe) ∧ has(giraffe, long_legs) ∧ is(giraffe, tall)

Parrot is a bird and is green in color.
bird(parrot) ∧ has(parrot, green_colour)
```
