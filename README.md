# Expert Systems (ES) & Knowledge Engineering - Mid-Length Revision

هذا الملف عبارة عن مراجعة متوسطة (حوالي 300 سطر) تحتفظ بكل التفاصيل والمصطلحات ولكن بشكل منظم ومنسق يسهل الحفظ والمراجعة للامتحان.

---

## 1. What is an Expert System (ES)?

**ES** is a branch of **Artificial Intelligence** concerned with the concepts and methods of **symbolic inference** (reasoning) by a computer — and how the knowledge used to make those inferences is represented inside the machine.

الـ ES بيعمل 3 حاجات أساسية:
1. يحاكي قرارات الخبير البشري في مجال معين (Simulate expert decisions).
2. يجاوب على أسئلة ويوضح ويعالج الـ uncertainties.
3. يشتغل 24/7 من غير ما يتعب.

### How It Works (Main Components)
1. **Knowledge Base (KB):** المكان اللي بنخزن فيه كل الحقائق (Facts) والقواعد (Rules). ده عقل الخبير جوه الكمبيوتر.
2. **Inference Engine:** ده "المحرك" اللي بياخد المعطيات ويطبقها على الـ KB عشان يستنتج الحل (Reasoning). 
   - **Forward Chaining:** بيبدأ من البيانات (Data) لحد ما يوصل للنتيجة.
   - **Backward Chaining:** بيبدأ من النتيجة (Goal) ويرجع يشوف محتاج بيانات إيه عشان يثبتها.

---

## 2. Comparisons (مقارنات هامة جداً)

### Human Expert vs. Expert System
| Feature | Human Expert | Expert System |
|---|---|---|
| **Time Availability** | Workdays فقط | **Always (24/7)** |
| **Geographic** | Local | **Anywhere** |
| **Safety** | Irreplaceable (لا يعوض) | **Replaceable** |
| **Consumable** | Yes | **No** |
| **Performance** | Variable | **Consistent** |
| **Speed** | Variable | **Consistent (usually faster)** |
| **Cost** | High | **Reasonable** |

### Conventional Systems vs. Expert Systems
| Conventional Systems | Expert Systems |
|---|---|
| المعلومات والمعالجة في برنامج واحد مدمج | الـ KB منفصلة عن الـ Inference Engine |
| البرنامج لا يخطئ (عنده إجابة محددة) | ممكن يغلط (عشان بيبني على heuristics) |
| محتاج كل الـ input data عشان يشتغل | يقدر يشتغل بمعلومات غير مكتملة (Incomplete) |
| الهدف الرئيسي: **Efficiency** | الهدف الرئيسي: **Effectiveness** |
| يعتمد على: Numerical representation | يعتمد على: Symbolic representation |

---

## 3. History & When to use ES
- **Edward Feigenbaum:** (جامعة Stanford) هو "أبو الـ Expert Systems".
- **John McCarthy:** (MIT) اخترع لغة **LISP** للذكاء الاصطناعي.
- الأنظمة القديمة المشهورة (1960s-1970s): **DENDRAL, MYCIN, XCON**.

**امتى بنحتاج نبني ES؟**
- الخبراء مش متاحين أو مش دايما reliable.
- البيئة المحيطة خطيرة (Hazardous).
- بنحتاج Second Opinion.
- المهمة تعتمد على الـ Reasoning مش مجرد reflexes.

---

## 4. Advantages & Disadvantages

**المميزات (Advantages):**
- **Permanence:** لا ينسى المعرفة، الخبير البشري ينسى أو يموت.
- **Reproducibility:** سهل تعمل منه ألف نسخة بتكلفة قليلة جداً.
- **Efficiency:** غالي في البناء، لكن رخيص جداً في التشغيل.
- **Documentation & Explanation:** بيوثق كل خطوة ويشرح أسباب قراراته.
- **Completeness & Consistency:** بيراجع كل البيانات بنفس الكفاءة دايماً دون تأثير بالمزاج.

**العيوب (Disadvantages):**
- **Knowledge Acquisition Bottleneck:** أصعب خطوة هي سحب الخبرة من رأس الخبير.
- **Degradation:** لما المشكلة تخرج برا مجاله بيعك، مش بيعرف يقول "معرفش".
- **No Common Sense:** معندوش بديهيات.
- **No Creativity:** مش بيعرف يبتكر حلول لمشاكل غير مألوفة.
- **No Self-learning:** لازم حد يحدثه.

---

## 5. Additional ES Components & Types

### Mores Components
- **User Interface:** صلة الوصل بين المستخدم والنظام.
- **Working Memory:** بيخزن الـ Data الخاصة بالمشكلة الحالية فقط (e.g., `loves(Hala, eggs)`).
- **Explanation:** بيوريك إزاي وصل للنتيجة (Tracing rules).
- **Justification:** بيشرح "ليه" النتيجة دي صحيحة ومبرراتها.

### Types of ES
1. **Rule-Based ES:** بيستخدم (IF-THEN) rules. الأكثر شيوعاً.
2. **Fuzzy Logic ES:** يتعامل مع العبارات الغامضة (مثل "حار جداً").
3. **Knowledge-Based ES:** يحاكي طريقة تفكير الخبير.
4. **Neural Networks ES:** يتعلم من البيانات زي المخ (Speech/Image recognition).

### Applications
- **Diagnosis:** تشخيص الأمراض أو الأعطال (مثل MYCIN).
- **Design:** تصميم أنظمة (مثل DENDRAL).
- **Monitoring:** مراقبة البيانات (مثل REACTOR).
- **Interpretation:** استنتاج بيانات حساسات (مثل PROSPECTOR).
- **Debugging & Repair:** حل المشاكل خطوة بخطوة (مثل MACSYMA).

---

## 6. Development Tools & Participants

**المشاركون:**
1. **Expert:** مصدر المعرفة (Domain Expert).
2. **Knowledge Engineer:** المهندس اللي بيقعد مع الخبير ويحول كلامه لـ Rules يفهمها الكمبيوتر.
3. **User:** المستخدم النهائي (يُشارك في تقييم النظام).

**أدوات التطوير:**
- اللغات الخوارزمية: C, Pascal.
- اللغات الرمزية (Symbolic): **Prolog, LISP**.
- بيئات التطوير: Art, KEE.
- قوالب الأنظمة (Shells): **JESS, CLIPS**.

---

# Knowledge Base & Knowledge Engineering (KE)

---

## 7. Data vs. Information vs. Knowledge

- **Data (البيانات):** أرقام وحقائق خام مجردة بدون معنى. `(مثال: 38.5)`
- **Information (المعلومات):** بيانات تم تنظيمها لتوضيح معنى. `(مثال: الحرارة 38.5°C)`
- **Knowledge (المعرفة):** معلومة أضيف إليها الغرض والقدرة على التصرف. `(مثال: حرارة عالية تعني عدوى وتحتاج علاج)`

**اتجاهات الهرم المعرفي:**
- من أسفل لأعلى: Data → Information → Knowledge.
- من أعلى لأسفل (Reversed): Knowledge → Information → Data (لازم أكون خبير عشان أعرف أجمع البيانات الصح).

---

## 8. Explicit vs. Tacit Knowledge

| Explicit Knowledge (صريحة) | Tacit Knowledge (ضمنية) |
|---|---|
| **Know-what** | **Know-how** |
| Formalized & codified (مكتوبة بشكل رسمي) | في دماغ الشخص (لا تكتب بكلمات أو أرقام بسهولة) |
| سهل تخزينها ونقلها (Books, Databases) | صعب جداً نقلها وتخزينها (Intuition, Skills) |

**Conversion 4 Methods (طرق التحويل):**
1. **Externalization:** من Tacit إلى Explicit (خبير بيكتب كتاب أو تقرير).
2. **Combination:** من Explicit إلى Explicit (دمج كتابين لمعلومة جديدة).
3. **Internalization:** من Explicit إلى Tacit (طبيب بيقرأ ويطبق كتير فتتحول لخبرته الشخصية).
4. **Socialization:** من Tacit إلى Tacit (واحد بيقعُد مع خبير وبيتعلم منه بالممارسة).

---

## 9. Knowledge Engineering (KE) & Activities

**التعريف:** هي عملية استخراج، تنظيم، وتمثيل الخبرة وتحويلها وصيانتها جوه الـ Knowledge Base.
ولها نظرتين: 
- **Narrow View:** التعامل مع المعرفة فقط جوه النظام (Acquisition, Representation, Inferencing, Validation).
- **Broad View:** دورة حياة الذكاء الاصطناعي كلها (تصميم، بناء، صيانة وإدارة النظام).

### Activity 1: Knowledge Acquisition (جمع المعرفة)
أصعب مرحلة (Bottleneck). بتتم على 5 مراحل: Identification → Conceptualization → Formalization → Implementation → Testing.

**طرق التجميع (Methods):**
1. **Manual:** مقابلات مع الخبير والمراقبة (Interviewing, Observing). مكلفة وبطيئة.
2. **Semi-Automatic:** ببرامج تساعد الخبير يسجل معلوماته بنفسه.
3. **Automatic:** (Machine Learning) النظام بيتعلم من البيانات الجاهزة.

**الصعوبات:** الخبير مبيعرفش يشرح الخطوات، المعرفة متوزعة مبعثرة، أو الخبير بيغير سلوكه قدام الـ Knowledge Engineer (رد فعل المراقبة).

---

### Activity 2: Knowledge Representation (KR) (تمثيل المعرفة)
الـ Procedural Code (زي C++ و Java) مش مناسبين. بنستخدم طرق مخصصة:

#### 1. Logical Representations
تعتمد على Syntax (رموز) و Semantics (معاني).
- **Propositional Logic (Sentential):** قواعد بسيطة Declarative (صح أو غلط).
  مثال: `P ∧ Q ⇒ R` (لو P و Q صح، إذن R صح).
  محدودة التعبير.
- **First-Order Logic (FOL):** أدق لأنها تستخدم المتغيرات والـ Quantifiers:
  - **Universal (∀):** For All (للكل). 
    مثال: `∀x bird(x) → animal(x)` (كل الطيور حيوانات).
  - **Existential (∃):** There Exists (يوجد على الأقل واحد).
    مثال: `∃x younger(x, Haneen)` (فيه حد أصغر من حنين).

#### 2. Semantic Networks (الشبكات الدلالية)
رسمة Graph تتكون من:
- **Nodes:** أشياء أو مفاهيم (مثال: طائر، حيوان).
- **Arcs:** العلاقات اللي بتربطهم (مثال: is-a, has-a).
طبيعية بالنسبة للتفكير البشري.

#### 3. Production Rules (قواعد الإنتاج IF-THEN)
- `IF (Condition) THEN (Action/Conclusion)`.
- **مميزات:** Modular (مستقلة وسهلة التعديل)، مرنة جداً.
- **عيوب:** لو القواعد بقت آلاف، النظام بيبقى بطيء.

#### 4. Frames (الإطارات)
هيكل تنظيمي شبه الـ Classes في البرمجة.
- كل Frame يحتوي على **Slots** (Attributes & Values).
- بتساعد في الوراثة (**Inheritance**) وحل المشاكل بالـ **Matching**.

### مقارنة سريعة لطرق الـ KR:
| Scheme | Pros | Cons |
|---|---|---|
| **Rules** | سهل يتفهم، Modular | بطيء لما المشكلة تكبر |
| **Semantic Nets** | سهل تتبع العلاقات والوراثة | أحيانا مبهم (Ambiguous) |
| **Frames** | معبر جداً لخصائص الكيانات | برمجته صعبة ومكلفة |
| **Logic** | مثبت رياضياً وصحيح دائماً | بطيء جداً مع البيانات الكبيرة |

---

### Activity 3: Validation & Verification (V&V)
- **Verification:** (هل بنينا النظام صح؟ Building the system right) نتأكد إن القواعد مضبوطة داخلياً ومفيش تعارض.
- **Validation:** (هل بنينا النظام المطلوب للعميل؟ Building the right system) نتأكد إن الحل بيحل مشكلة المستخدم فعلاً والمخرجات مقبولة عملياً.

---

## 10. Important Logics Examples (Examples directly from material)

ركز على أمثلة الـ First Order Logic لأنها بتيجي كتير:

- جميع البشر والحيوانات والطيور يتنفسون ويأكلون ويعتبرون كائنات حية:
```
∀X [[human(X) ∨ animal(X) ∨ bird(X)] ∧ eat(X) ∧ breath(X)] → living(X)
```

- كل الطيور حيوانات وممكن تطير:
```
∀X bird(X) → animal(X) ∧ canfly(X)
```

- كل رجل أو امرأة ليهم رجلين يبقوا بشر:
```
∀X [[man(X) ∧ haslegs(X,2)] ∨ [woman(X) ∧ haslegs(X,2)]] → human(X)
```

- القطة حيوان ولديها فرو (هنا Propositional بدون شمول لأننا بنتكلم عن القطة فقط):
```
animal(cat) ∧ has(cat, fur)
```

- لا يوجد فطر بنفسجي سام (استخدام الـ Existential في النفي):
```
¬∃x purple(x) ∧ mushroom(x) ∧ poisonous(x)
```
