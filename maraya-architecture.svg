import React from 'react';

// ملف React واحد يعرض مخطط معماري مرئي لمنصة "مرايا" مع شروحات.
// يُستخدم TailwindCSS للتصميم. هذا مكون جاهز للعرض والمعاينة.

export default function MarayaArchitectureDiagram() {
  return (
    <div dir="rtl" className="p-6 bg-gray-50 min-h-screen font-sans text-gray-800">
      <header className="mb-6">
        <h1 className="text-3xl font-bold">مخطط معماري تفصيلي — منصة "مرايا"</h1>
        <p className="mt-2 text-sm text-gray-600">مخطط مرئي يوضح الأجزاء، المكونات، علاقاتها، وتدفق البيانات بين المستخدمين، القنوات، المجموعات، الصفحات، وقاعدة البيانات، مع ملاحظات لتوليد اقتراحات ذكية.</p>
      </header>

      <main className="grid grid-cols-1 lg:grid-cols-2 gap-6">
        {/* الرسم البياني */}
        <section className="bg-white rounded-2xl shadow p-4">
          <div className="mb-3">
            <h2 className="text-xl font-semibold">الرسم البياني العام</h2>
            <p className="text-sm text-gray-500">انقر لتكبير أو استخدم معاينة كاملة للشكل.</p>
          </div>

          <div className="overflow-auto">
            <svg width="1200" height="900" viewBox="0 0 1200 900" xmlns="http://www.w3.org/2000/svg">
              <defs>
                <filter id="soft" x="-20%" y="-20%" width="140%" height="140%">
                  <feDropShadow dx="0" dy="4" stdDeviation="8" floodColor="#000" floodOpacity="0.08"/>
                </filter>
              </defs>

              {/* Users cluster */}
              <rect x="40" y="40" rx="14" ry="14" width="370" height="220" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="60" y="72" fontSize="18" fontWeight="700">المستخدمون وواجهة العميل</text>

              <g>
                <rect x="60" y="92" rx="10" width="140" height="48" fill="#FAFAFA" stroke="#E6EEF7" />
                <text x="75" y="122" fontSize="12">تسجيل الدخول / Auth</text>

                <rect x="210" y="92" rx="10" width="200" height="48" fill="#FAFAFA" stroke="#E6EEF7" />
                <text x="230" y="122" fontSize="12">الملف الشخصي (Profile)</text>

                <rect x="60" y="152" rx="10" width="350" height="48" fill="#FEFEFE" stroke="#E6EEF7" />
                <text x="75" y="182" fontSize="12">تطبيقات: ويب - أندرويد - iOS - API للجهات الخارجية</text>
              </g>

              {/* Social Graph / Relationships */}
              <rect x="440" y="40" rx="14" ry="14" width="360" height="220" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="460" y="72" fontSize="18" fontWeight="700">العلاقات الاجتماعية & التفاعل</text>

              <g>
                <rect x="460" y="92" rx="10" width="160" height="40" fill="#FBFBFF" stroke="#DDE9FF" />
                <text x="480" y="118" fontSize="12">الأصدقاء / المتابعون (Graph DB)</text>

                <rect x="630" y="92" rx="10" width="180" height="40" fill="#FBFBFF" stroke="#DDE9FF" />
                <text x="650" y="118" fontSize="12">القنوات / الصفحات / المجموعات (Ownership)</text>

                <rect x="460" y="142" rx="10" width="350" height="40" fill="#FEFEFF" stroke="#DDE9FF" />
                <text x="480" y="168" fontSize="12">الأنشطة: منشورات، تعليقات، تفاعلات (Like, Share, Save)</text>
              </g>

              {/* Feed & Recommendation */}
              <rect x="40" y="290" rx="14" ry="14" width="360" height="240" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="60" y="320" fontSize="18" fontWeight="700">خدمة الخلاصات (Feed) و التوصية</text>

              <g>
                <rect x="60" y="350" rx="10" width="160" height="40" fill="#FFF8F0" stroke="#F3E7D6" />
                <text x="80" y="374" fontSize="12">Feed Generator (قواعد توقيتية + محركات ترشيح)</text>

                <rect x="230" y="350" rx="10" width="170" height="40" fill="#FFF8F0" stroke="#F3E7D6" />
                <text x="252" y="374" fontSize="12">Recommendation Engine (ML — Graph + Content + Behavior)</text>

                <rect x="60" y="402" rx="10" width="340" height="48" fill="#FFFDFE" stroke="#F3E7D6" />
                <text x="80" y="430" fontSize="12">Personalization & Signals: interests, history, social signals, recency</text>
              </g>

              {/* Backend Services */}
              <rect x="440" y="290" rx="14" ry="14" width="360" height="240" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="460" y="320" fontSize="18" fontWeight="700">خدمات الباك-إند & البنية التحتية</text>

              <g>
                <rect x="460" y="350" rx="10" width="160" height="40" fill="#F7FFF7" stroke="#DFF7E6" />
                <text x="480" y="374" fontSize="12">API Gateway & Auth Service</text>

                <rect x="630" y="350" rx="10" width="160" height="40" fill="#F7FFF7" stroke="#DFF7E6" />
                <text x="650" y="374" fontSize="12">Realtime (WebSocket / RTC) & Message Broker</text>

                <rect x="460" y="402" rx="10" width="330" height="40" fill="#F7FFF7" stroke="#DFF7E6" />
                <text x="480" y="428" fontSize="12">Workers / Background Jobs (Notifications, Media processing)</text>
              </g>

              {/* Storage and DBs */}
              <rect x="840" y="40" rx="14" ry="14" width="280" height="240" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="860" y="72" fontSize="18" fontWeight="700">قاعدة البيانات و التخزين</text>

              <g>
                <rect x="860" y="100" rx="8" width="240" height="40" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="126" fontSize="12">User DB (SQL — profiles, auth)</text>

                <rect x="860" y="148" rx="8" width="240" height="40" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="174" fontSize="12">Graph DB (Neo4j / Janus — علاقات اجتماعية)</text>

                <rect x="860" y="196" rx="8" width="240" height="40" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="222" fontSize="12">Feed DB / Cache (Redis, Materialized Views)</text>

                <rect x="860" y="244" rx="8" width="240" height="40" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="270" fontSize="12">Media Storage (Object Storage + CDN)</text>
              </g>

              {/* Analytics & Moderation */}
              <rect x="840" y="310" rx="14" ry="14" width="280" height="160" fill="#fff" stroke="#E5E7EB" filter="url(#soft)" />
              <text x="860" y="338" fontSize="16" fontWeight="700">تحليلات / مراقبة / أمن</text>

              <g>
                <rect x="860" y="364" rx="8" width="240" height="36" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="388" fontSize="12">Analytics DB / Event Store (Clickstream)</text>

                <rect x="860" y="406" rx="8" width="240" height="36" fill="#FFF" stroke="#E6EEF7" />
                <text x="880" y="430" fontSize="12">Moderation & Safety (ML + Human-in-loop)</text>
              </g>

              {/* Arrows (simplified) */}
              <defs>
                <marker id="arrow" markerWidth="8" markerHeight="8" refX="6" refY="4" orient="auto">
                  <path d="M0,0 L8,4 L0,8 z" fill="#94A3B8" />
                </marker>
              </defs>

              {/* Users -> API Gateway */}
              <line x1="240" y1="250" x2="520" y2="300" stroke="#94A3B8" strokeWidth="2" markerEnd="url(#arrow)" />
              <text x="300" y="270" fontSize="11">طلبات API / WebSocket</text>

              {/* Backend -> DBs */}
              <line x1="660" y1="420" x2="860" y2="340" stroke="#94A3B8" strokeWidth="2" markerEnd="url(#arrow)" />
              <text x="740" y="380" fontSize="11">قراءة/كتابة</text>

              {/* Feed -> User */}
              <line x1="220" y1="450" x2="320" y2="320" stroke="#94A3B8" strokeWidth="2" markerEnd="url(#arrow)" />
              <text x="240" y="400" fontSize="11">خلاصات مخصصة</text>

              {/* Graph -> Recommendation */}
              <line x1="740" y1="120" x2="410" y2="370" stroke="#94A3B8" strokeWidth="2" markerEnd="url(#arrow)" />
              <text x="560" y="210" fontSize="11">إشارات اجتماعية للسيرفر التوصية</text>

              {/* Moderation -> Feed */}
              <line x1="980" y1="420" x2="380" y2="420" stroke="#94A3B8" strokeWidth="2" markerEnd="url(#arrow)" />
              <text x="700" y="440" fontSize="11">قواعد المحتوى/فلترة</text>

            </svg>
          </div>
        </section>

        {/* الشروحات والشرح التفصيلي */}
        <section className="bg-white rounded-2xl shadow p-6">
          <h2 className="text-xl font-semibold mb-3">تفسير مُفَصَّل وعمليات الربط</h2>

          <div className="prose prose-sm text-right">
            <h3>1. مكونات رئيسية</h3>
            <ul>
              <li><strong>الواجهة/العميل:</strong> تطبيقات الويب والموبايل تتواصل عبر API Gateway وRealtime endpoints.</li>
              <li><strong>Authentication & Profiles:</strong> خدمة التوثيق تخزن في قواعد SQL مع ارتباط للهوية.</li>
              <li><strong>Graph DB:</strong> تخزن علاقات الأصدقاء/المتابعين، والعضويات في القنوات/المجموعات/الصفحات. ممتازة للاستعلامات الارتباطية.</li>
              <li><strong>Feed & Recommendation:</strong> مزيج من قواعد منطقية (Heuristics) ومحركات ML تستخدم إشارات: سلوك، تفضيلات، علاقات اجتماعية، زمنية، محتوى.</li>
              <li><strong>Media & CDN:</strong> ملفات الفيديو والصور تُخزن كـ objects وتُقدم من CDN لخفض زمن التحميل.</li>
              <li><strong>Workers & Message Broker:</strong> مهام المعالجة الخلفية (ترميز فيديو، تحليل نصي، إشعارات) تعمل على صفوف رسائل (Kafka/Rabbit).</li>
              <li><strong>Analytics & Moderation:</strong> تجمع الأحداث (events) لمعالجة التحليلات وإنذار السلوك المسيء وتهيئة المراجعة البشرية.</li>
            </ul>

            <h3>2. علاقة المستخدمين ببعض</h3>
            <p>علاقات المستخدمين (أصدقاء، متابعون) تمثل كـ graph: كل مستخدم هو عقدة (node) والروابط تمثل نوع العلاقة (متابع، صديق، محظور...). تُخزن هذه البيانات في Graph DB لتسهيل استعلامات مثل: "أصدقاء المشتركين الذين شاهدوا هذا الفيديو" أو "اقتراح أصدقاء".</p>

            <h3>3. القنوات، المجموعات، والصفحات</h3>
            <p>كل قناة/مجموعة/صفحة تمثل كائنًا (entity) مرتبطًا بمالك/مشرفين ومجموعة من العضويات. يمكن للعلاقات أن تكون: عضوية مباشرة، دعوة، طلب، وانضمام تلقائي حسب قواعد. يتم تخزين العضويات أيضًا في Graph DB أو كجزء من User DB مع مفهرس (index) للبحث السريع.</p>

            <h3>4. إدارة وتوصيل العلاقات إلى قاعدة البيانات</h3>
            <ol>
              <li><strong>أحداث المستخدم (Events):</strong> كل تفاعل (منشور، تعليق، متابعة) يولد حدثًا يدفعه العميل إلى API Gateway.</li>
              <li><strong>المعالجة الفورية:</strong> لبعض الحالات (مثل الرسائل والمكالمات) يُستخدم Realtime Service (WebSocket/RTC) للتوصيل الفوري.</li>
              <li><strong>الكتابة المهيكلة:</strong> بيانات الهوية تُخزن في SQL، والعلاقات والعضويات في Graph DB، والـ feeds الموادية في قواعد عرض (materialized views) أو Redis للقراءات السريعة.</li>
              <li><strong>التجهيز والخلفية:</strong> مهام مثل ترميز الفيديو وفحص المحتوى تُرسل إلى صفوف الرسائل وتُعالج بواسطة Workers.</li>
            </ol>

            <h3>5. كيف تُولّد الاقتراحات الذكية (Recommendation)</h3>
            <p>نظام التوصية يجمع إشارات متعددة:</p>
            <ul>
              <li>السلوك الفردي (تصفح، تفاعلات، وقت مشاهدة).</li>
              <li>العلاقات الاجتماعية (ما يعجبه أصدقاؤه، ما تعجب به مجموعاته).</li>
              <li>الميزات النصية/المرئية للمحتوى (الوسوم، التصنيف، مواضيع الفيديو).</li>
              <li>الزمن (الجديدية، الأحداث الفورية).</li>
            </ul>
            <p>خط سير عمل سريع: جمع إشارات → بناء صفوف سمات (feature vectors) → تقييم عبر نماذج ML (ranking) → تطبيق قواعد تجارية (business rules) → عرض على المستخدم (A/B testing + اشرح سبب الاقتراح إذا لزم).</p>

            <h3>6. مثال تدفق: مستخدم ينشر مشاركة</h3>
            <ol>
              <li>العميل يرسل POST للمشاركة إلى API Gateway.</li>
              <li>الخدمة تحفظ المدخل في Post DB وتدفع حدثًا إلى Message Broker.</li>
              <li>Workers تقوم بفحص المحتوى (Moderation), توليد المقتطفات، ترميز الوسائط، وتحديث Search Index.</li>
              <li>Feed Generator يقوم بترشيح المنشور للأشخاص المناسبين بناءً على العلاقات والإشارات، ويحدث Materialized Views أو يخزن إشعارات في Redis/Feed DB.</li>
            </ol>

            <h3>7. تدابير الأمان والخصوصية</h3>
            <ul>
              <li>تشفير بيانات حساسة في الراحة (at rest) والناقلة (in transit).</li>
              <li>تصميم صلاحيات دقيقة للمشرفين والمالكين والعضويات.</li>
              <li>حماية واجهات API بمعدلات طلبات (rate limiting) وجدران تطبيق (WAF).</li>
              <li>نظام مراجعة محتوى مختلط (ML + إنسان) مع إمكانية الطعن والاستئناف.</li>
            </ul>

            <h3>8. ملاحظات هندسية وإقتراحات عملية</h3>
            <ul>
              <li>استخدم Graph DB لعلاقات الشبكة الاجتماعية (Neo4j, JanusGraph) مع SQL للهوية والبيانات الطولية.</li>
              <li>اعمل Materialized Feeds للقراءات السريعة، واهتم بالـ cache (Redis) لخفض زمن الاستجابة.</li>
              <li>صمم نظام توصية هجيني: Retrieval (البحث الأولي) + Ranking (تصنيف) لتوفير سرعة وجودة.</li>
              <li>اعتمد بنية Microservices مع API Gateway وService Mesh لاحقًا (Istio) للتوزيع والأمان.</li>
            </ul>

            <h3>9. ماذا ترى في المخطط (مفتاح سريع)</h3>
            <ul>
              <li>المستطيلات الكبيرة: مكونات/خدمات رئيسية.</li>
              <li>المستطيلات الصغيرة: خدمات ضمنية أو قواعد بيانات.</li>
              <li>الأسهم: تدفق البيانات/طلبات.</li>
            </ul>

            <p className="mt-4 text-sm text-gray-500">هل تريد نسخة قابلة للطباعة (PDF) من هذا المخطط؟ أم تفضّل أن أصدّر هذا الرسم كصورة PNG بوضوح عالٍ مع نسخة عربية بالعرض الكامل؟</p>
          </div>
        </section>
      </main>

    </div>
  );
}
