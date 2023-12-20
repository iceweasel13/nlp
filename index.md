**_Doğal Dil İşleme Teknolojileri ve Günlük Hayattaki Uygulamaları_**

**HAZIRLAYAN**

**Adı Soyadı:** Nihat Zaman

**Öğrenci Numarası :** 190303030

**Teslim tarihi :** 20/12/2023

**DERS ADI :** Doğal Dil İşlemeye giriş

**DERS YÜRÜTÜCÜSÜ :** İbrahim Arı

# Giriş

Doğal Dil İşleme (NLP), bilgisayarlar ve insan dili arasındaki etkileşimi inceleyen yapay zekanın heyecan verici bir alt alanı olarak ortaya çıkmıştır. İlk adımları 1950'lerde atılan NLP, o dönemde sınırlı bilgisayar gücü ve gelişmemiş algoritmalar nedeniyle oldukça ilkel düzeydeydi. Ancak zamanla, dilbilim ve bilgisayar bilimlerinin kesişimi olarak gelişerek, bilgisayarların insan dilini anlaması ve işlemesi konusunda devrim niteliğinde ilerlemeler kaydetmiştir.

NLP'nin ilk önemli başarısı, 1950'lerin sonunda gerçekleşen otomatik çeviri çalışmalarıydı. Bu dönemde, bilgisayarların basit metinleri bir dilden diğerine çevirebilmesi büyük bir yenilik olarak görüldü. 1960'lardan 1980'lere kadar, kural tabanlı sistemler ve dilbilimsel kurallar üzerine yoğunlaşıldı. Bu dönemde NLP, temel dilbilgisel yapıları tanıma ve işleme kapasitesine sahip oldu.

1990'larda, istatistiksel modellerin ve makine öğreniminin yükselişiyle NLP'de yeni bir dönem başladı. Büyük veri setleri ve gelişmiş algoritmalar sayesinde, NLP sistemleri daha karmaşık dil yapılarını anlayabilir ve doğal dilde daha akıcı işlemler gerçekleştirebilir hale geldi. Bu dönem, konuşma tanıma ve otomatik çeviri gibi uygulamaların gelişiminde önemli bir rol oynadı.

21.yüzyıla gelindiğinde, derin öğrenme ve yapay sinir ağları, NLP'nin sınırlarını daha da genişletti. Özellikle GPT-4 ve BERT gibi büyük dil modellerinin gelişimi, metin üretimi, duygu analizi ve dil anlama konularında çığır açıcı yenilikler getirdi. Bu modeller, dilin daha ince nüanslarını anlayarak ve öğrenerek insan benzeri bir doğal dil işleme kabiliyeti sunmaktadır.
Günümüzde, NLP teknolojileri, sesli asistanlardan sosyal medya analizlerine, otomatik özetlemelerden duygu tespitine kadar geniş bir yelpazede günlük hayatımıza entegre olmuş durumdadır. Akıllı telefonlardan sosyal platformlara, müşteri hizmetlerinden sağlık sektörüne kadar birçok alanda karşımıza çıkan NLP, sürekli gelişen algoritmalar ve artan veri erişimiyle insan-makine etkileşimini yeniden şekillendiriyor. NLP'nin geleceği, sadece teknolojik ilerlemelerle sınırlı kalmayıp, etik, sosyal ve kültürel açılardan da derin etkiler yaratma potansiyeline sahiptir.

## NLP İşleyişi ve Temel Kavramlar##

Bilgisayarların konuştuğumuz dili anlayabilmesi için elde edilen veriler bir dizi temel süreçten geçmektedir. Bu bölümde, doğal dil işlemenin temel adımlarına ve kavramlarına değinilecektir.

1.**Tokenization**

Bir metni daha küçük birimlere, genellikle kelimeler veya cümlelere bölme işlemidir. Bu birimler, NLP görevlerinde daha sonraki analizler için temel yapı taşları olarak kullanılır.

**Örnek:** "Kedi ve köpek matın üzerinde uyuyor."

**Tokenlar:** ["Kedi","ve", "köpek" "matın", "üzerinde", "uyuyor","."]

2.**Metin Temizleme**

Verinin parçalara ayrılmasının ardından ortaya çalışma için gerekli olmayan parçalar ortaya çıkabilmektedir.Bu gerekli olmayan yapılardan kurtulmak için metin temizleme adımı gerçekleştirilmektedir. Bu işlemin amacı metni noktalama işaretlerinden ve özel karakterlerden
arındırarak daha temiz bir veri elde etmektir.

**Örnek:** ["Kedi","ve", "köpek" "matın", "üzerinde", "uyuyor","."]

**Çıktı:** ["Kedi","ve", "köpek" "matın", "üzerinde", "uyuyor"]

3.**Metin Normalleştirme**
Metin normalleştirme, Doğal Dil İşleme (NLP) çalışmalarında kritik bir öneme sahiptir ve bu süreç, metni işlemeye daha uygun hale getirir. Normalleştirme, metnin farklı bağlamlarda standart bir forma dönüştürülmesini ifade eder ve birçok farklı işlemi içerebilir. Bunlar arasında, yinelenen boşlukların ve noktalama işaretlerinin kaldırılması, metindeki vurgu işaretlerinin çıkarılması, büyük harflerin küçük harfe dönüştürülmesi yer alır. Ayrıca, özel karakterlerin ve emojilerin kaldırılması veya dönüştürülmesi, sayıların rakamla ifade edilmesi, kısaltmaların açık halleriyle yazılması gibi işlemler de bu sürece dahildir. Tarih biçimlerinin ve diğer standart veri formatlarının düzenlenmesi, yazım hatalarının düzeltilmesi ve nadir kullanılan kelimelerin daha yaygın eş anlamlılarıyla değiştirilmesi de normalleştirme sürecinin bir parçasıdır. Normalleştirme işlemlerinin hangilerinin uygulanacağı, ele alınan iş probleminin doğasına ve ihtiyaçlarına bağlı olarak değişiklik gösterir. Bu kararları veri bilimciler, projenin hedefleri ve verinin özellikleri doğrultusunda alır. Doğru normalleştirme tekniklerinin uygulanması, NLP modellerinin daha etkili ve doğru sonuçlar üretmesini sağlar ve veri üzerindeki potansiyel hataların önüne geçer.

4.**Gövdeleme (Stemming) ve Kök Bulma (Lemmatization)**
Gövdeleme ve kök bulma işlemleri ön işleme basamaklarından biridir. Bu aşamanın amacı bir metindeki her bir kelimeden eklerin kaldırılması işlemidir.

5.**Önemsiz kelimeler (Stop Words)**
Önemsiz kelimeler verinin daha iyi işlenebilmesi için gerçekleştirilmesi gereken ön adımlardan birisidir. Bu işlem kısaca dilde yaygın kullanılan ve metnin anlamı üzerinde etkisi olmayan kelimelerin veriden çıkarılması ile gerçekleştirilir. Örneğin Türkçede yer alan ve, ama, ki gibi ifadeler bu kapsam altında değerlendirilebilir.

## Metin Öznitelik Çıkarımı##

Ön işleme tamamlanmasının ardından veriden öznitelik çıkarım aşamasına geçilir. Bu aşama kısaca veri içerisindeki belirli bir özellik veya niteliğin belirlenmesi olarak söylenebilir.

### Kelime Çantası Modeli

Kelime çantası modeli, metinlerden özellik çıkarma yollarından bir tanesidir. Bu model bir belgedeki kelimelerin oluşumunu örneğin,terim sayılarını, açıklayan metnin bir temsilidir. Bilinen kelimelerden kelime haznesi oluşturulur, buna “kelime çantası” denir. Model, bir kelimenin belgenin neresinde olduğu ile değil, sadece belgede bulunup bulunmadığı ile ilgilenir.

### TF-IDF (Term Frequency-Inverse Document Frequency) Yöntemi

TF-IDF, Doğal Dil İşleme (NLP) ve metin madenciliğinde yaygın olarak kullanılan bir yöntemdir. Bu yöntem, bir kelimenin bir dokümanda ne kadar önemli olduğunu belirlemek için kullanılır. TF-IDF, iki temel bileşenden oluşur:

**Term Frequency (TF):**
Bir kelimenin bir dokümanda ne sıklıkta geçtiğini ifade eder. Basitçe, bir kelimenin dokümandaki toplam kelime sayısına oranı olarak hesaplanır. TF, belirli bir kelimenin belgedeki önemini doğrudan ölçer.

**Inverse Document Frequency (IDF):** Bir kelimenin tüm doküman koleksiyonunda ne kadar nadir olduğunu ölçer. Bir kelimenin birçok dokümanda geçmesi durumunda, bu kelime genel olarak daha az önemli kabul edilir. IDF, her kelimenin tüm dokümanlarda ne sıklıkta geçtiğinin ters logaritması alınarak hesaplanır.

TF-IDF değeri, bu iki ölçütün çarpımı olarak elde edilir. Yüksek TF-IDF değerine sahip kelimeler, belirli bir doküman için daha önemli kabul edilirken, düşük TF-IDF değerine sahip kelimeler daha az önemli veya yaygın kelimeler olarak değerlendirilir. Bu yöntem, metinler arasındaki farklılıkları belirlemede, anahtar kelime çıkarmada ve dokümanların otomatik sınıflandırılmasında etkili bir araçtır. TF-IDF, özellikle arama motorları ve bilgi geri kazanım sistemlerinde yaygın olarak kullanılmaktadır.

# Günlük Hayatta Doğal Dil İşlemenin Yeri

Doğal Dil İşleme (NLP) teknolojileri, günlük yaşamımızın birçok alanında önemli bir rol oynar. İletişimden bilgi erişimine, eğlenceden iş dünyasına kadar geniş bir yelpazede uygulamalar bulunmaktadır.

## Sosyal Medya Analizi ve Duygu Analizi##

NLP, sosyal medya gönderilerini, yorumlarını ve incelemelerini analiz ederek kullanıcıların duygularını, tutumlarını ve tercihlerini belirlemek için kullanılır. Bu, markaların müşteri geri bildirimlerini anlamalarını ve hedef kitleleriyle daha etkili bir şekilde iletişim kurmalarını sağlar.

**Örnek:** Marka izleme, kriz yönetimi, pazar araştırmaları ve ürün geliştirme stratejileri.

## Otomatik Metin Özetleme ve Öne Çıkarılmış İçerik Oluşturma

Otomatik özetleme teknolojileri, uzun metinleri kısa ve öz özetlere dönüştürerek, büyük bilgi miktarlarını hızlı ve etkili bir şekilde tüketilmesini sağlar.

**Örnek:** Akademik makalelerin özetlenmesi, haber özetleri ve iş raporlarının hazırlanması.

Bu uygulamalar, NLP'nin nasıl bir dizi pratik ve değerli araçlar sunduğunu ve günlük hayatımızı nasıl dönüştürdüğünü göstermektedir. NLP teknolojileri, insanların bilgiye erişimini kolaylaştırırken, aynı zamanda iş dünyasında daha bilinçli kararlar alınmasını sağlamakta ve kişisel yaşamımızda konfor ve verimlilik sunmaktadır. Bu teknolojinin sürekli gelişimi, gelecekte daha da entegre ve kullanışlı çözümler sunma potansiyeline sahiptir.

# Finans Sektöründe NLP Kullanımı

Günümüzde işletmeler dijital çağın gereksinimlerini yakalabilmek için doğal dil işleme üzerinde büyük yatırımlar yapmaktadırlar. Finans sektörü içinde bulundurmuş olduğu verilerin yüksek doğruluğu sebebiyle doğal dil işlemeyi en sık kullanan alanlardan birisidir. Finansal hizmet sektöründe NLP, risk değerlendirmeleri, güvenilirlik analizi, sohbet botları, portföy seçimi, adlandırılmış varlık tanıma, duygu analizi, konuşma tanıma vb. dahil olmak üzere bir çok alanda kullanılmaktadır.

## Metin ve Duyguları Analiz Etme

Metinden niteliksel/içgörüsel yapılandırılmış veri çıkarma işlemi olan metin analitiğinin önemi finans sektöründe gün geçtikçe artmaktadır. Metin analitiğinin en yaygın hedeflerinden biri duygu analizidir. Bu, metnin bağlamını anlayarak altında yatan duyguyu belirlemek ve anahtar finansal varlıkları metinden çıkarmak için kullanılan bir tekniktir. Finansal duygu analizi, hem alan hem de amaç açısından duygu analizinden farklıdır. Duygu analizinin amacı bilginin temelde olumlu mu yoksa olumsuz mu olduğunu belirlemektir.Ancak, NLP'ye dayalı finansal duygu analizinin amacı piyasanın habere nasıl tepki vereceğini ve hisse senedi fiyatının düşüp düşmeyeceğini belirlemektir.

## Riskleri Değerlendirme

Bankacılık sistemlerinde, önceki harcama alışkanlıklarına ve önceki kredi ödeme geçmişi verilerine dayanarak etkili bir kredi kartı limitinin belirlenmesi zordur. NLP araçları, kredi riskini değerlendirirken çeşitli veri kaynaklarını kullanır; kredi süreci sırasında kredi veren veya borçlu duyguları gibi tutarsız bilgileri tespit edebilirler. Risk değerlendirme süreci, kredi anlaşmasından tarih, konum ve ilgili taraflar hakkında bilgi çıkarmada yardımcı olur.

## Verileri Yapılandırma

Tüccarlar, yatırım firmaları ve finans uzmanlarının analiz etmesi ve araştırması gereken finansal kaynaklar arasında analiz ve araştırma raporları, şirket dosyaları ve çeyrek gelir belgeleri bulunmaktadır.
Bu kayıtlar genellikle pdf, XML, HTML, web ve beslemeler gibi formatlarda saklanır ve bunları sıralamak zaman alıcı ve yorucudur.NLP, kullanılmayan verilerden faydalı bilgiler çıkarılmasına olanak tanır. Finansal işletmeleri etkileyebilecek sorunları veya kalıpları ele almak için yapılandırılmamış verileri, içeriği ve bilgileri analiz etmek üzere NLP modellerini eğitebilirsiniz, bu da stratejik planlama inşa etmek için derinlemesine ek içgörü sağlar ve karar verme sürecini etkileyebilir.

## Portföyleri Seçme ve Optimize Etme

Veri bilimi ve makine öğrenimi, finansal hisse senedi piyasalarında yatırım portföylerini tahmin edebilir.Geçmişten gelen veriler, bir ticaret döneminin başlangıcını ve bir portföyü tahmin etmek için kullanılabilir.
NLP, arzu edilen ve istenmeyen hisseleri filtrelemek için kullanılabilir.
Yatırımcılar, bu verileri kullanarak mevcut sermayelerini mevcut varlıklar arasında dağıtabilir ve zamanla değerini en üst düzeye çıkarabilirler.

## Hisse Senedi Davranışını Tahmin Etme

Finansal analiz için hisse senedi davranışını tahmin etmek, dalgalanan ve rastgele veriler nedeniyle zor bir görevdir ve uzun vadeli ve mevsimsel değişiklikler değerlendirmede önemli hatalara neden olabilir. Öte yandan, makine öğrenimi ile birleştirilen NLP, finansal zaman serileriyle çalışma konusundaki önceki yöntemlerden çok daha başarılıdır.Bu iki teknoloji bir araya geldiğinde, büyük miktarda veriyle etkili bir şekilde başa çıkar ve hisse senedi fiyatlarının ve eğilimlerinin oynaklığını tahmin etmeyi kolaylaştırır ve hisse senedi ticareti kararları için değerli bir araç olur.

## Müşterilerin Katılımını Raporlama

Finansal şirketler, müşteri verilerini anlamayı, kişiselleştirilmiş hizmetleri ve müşteri iletişimini gerektiren yüksek kaliteli hizmetler sunmalıdır.Bu, finans sektöründe hayati öneme sahiptir ve NLP araçları, bankaların müşterilerle iletişim kurduklarında önemli bilgiler sağlar.
NLP algoritmaları, müşterilerin problemlerini tahmin eder ve tanımlar, böylece bankalar bu sorunları ele almak için politikalar ve hizmetler geliştirebilir. Diğer finansal firmalar, NLP'ye dayalı kararlar alabilir ve bu da genel raporlama sürecini daha da hızlandırabilir.

## Muhasebe ve Denetimler

NLP, denetim sürecinde önemli bir avantaj elde etmek için kritiktir. Finans profesyonelleri, günlük işlemlerdeki anomaliyi doğrudan tanımlamak, odaklanmak ve görselleştirmek için NLP kullanabilirler. NLP ile işlemlerdeki düzensizlikleri ve nedenlerini belirlemek, önemli potansiyel riskleri ve olası dolandırıcılıkları, örneğin kara para aklamayı tespit etmek daha az zaman ve çaba gerektirir.

# Gelişen Trendler ve Doğal Dil İşlemenin Gelecekteki Potansiyeli

## GPT-4 ve Benzeri Büyük Dil Modellerinin Etkisi

GPT-4 (Generative Pre-trained Transformer 4) ve benzeri büyük dil modelleri, Doğal Dil İşleme (NLP) alanında önemli bir dönüm noktasıdır. GPT-4, OpenAI tarafından geliştirilen, 175 milyar parametre içeren son derece gelişmiş bir dil modelidir. Bu model, metin üretimi, çeviri, özetleme ve soru-cevap gibi birçok NLP görevini insan seviyesinde gerçekleştirebilmektedir.

Büyük dil modellerinin en dikkat çekici yönlerinden biri, az miktarda veya hiç özelleştirilmiş eğitim verisi gerektirmeden geniş bir yelpazede görevleri yerine getirebilmesidir. Bu özelliği, NLP uygulamalarını daha erişilebilir ve maliyet etkin hale getirir. Ayrıca, bu modeller karmaşık dil yapılarını ve nüansları anlama konusunda önemli bir yeteneğe sahiptir, bu da onları doğal dil anlama ve etkileşimde yeni bir çağa taşır.

## Doğal Dil İşleme Alanındaki Gelecekteki Trendler

NLP alanındaki gelecekteki trendler, sürekli gelişen teknolojiler ve artan veri erişilebilirliği ile şekillenmektedir. Bu trendlerden bazıları şunlardır:

1. **Daha Gelişmiş Dil Modelleri:** GPT-4 gibi modellerin başarısı, daha da gelişmiş dil modellerinin geliştirilmesine yol açacaktır. Bu modeller, daha doğru anlam çıkarımı ve metin üretimi yapabilecek, ayrıca farklı diller ve lehçeler arasında daha iyi çeviri yapabilecektir.

1. **Duygu Analizinin Gelişimi:** Duygu analizi, müşteri geri bildirimlerinden sosyal medya gönderilerine kadar geniş bir veri yelpazesinde kullanıcının duygusal durumunu daha doğru bir şekilde anlamak için geliştirilecektir.

1. **Otomasyon ve Kişiselleştirme:** NLP teknolojileri, iş süreçlerinde daha fazla otomasyona ve müşteri hizmetlerinde kişiselleştirilmiş deneyimlere olanak tanıyacak şekilde geliştirilecektir.

1. **Çokdilli ve Çok Kültürlü Uygulamalar:** NLP, çeşitli dilleri ve kültürel bağlamları daha iyi anlamak için geliştirilecek, bu da küresel çapta daha etkin iletişim ve anlayış sağlayacaktır.

# Doğal Dil İşlemenin Zorlukları ve Etik Sorunları

Doğal Dil İşleme (NLP) teknolojilerinin gelişimi, bir dizi teknik zorluk ve veri gizliliği ile etik konuları da beraberinde getirmektedir. Bu zorluklar ve konular, NLP'nin geleceğini şekillendirmede önemli rol oynamaktadır.

## **Teknik Zorluklar**

1. **Dil Çeşitliliği ve Karmaşıklığı:** Dünya üzerinde binlerce dil ve lehçe bulunmaktadır. Her bir dilin kendine has gramer yapısı, deyimleri ve kültürel bağlamları vardır. Bu çeşitlilik, NLP sistemlerinin tüm dillerde aynı seviyede performans göstermesini zorlaştırır.
1. Anlamın Kontekste Bağlılığı: Dil, sıklıkla bağlam üzerine kuruludur. NLP sistemleri, özellikle ironi, mizah veya mecaz anlam gibi bağlamla yakından ilişkili dil kullanımlarını anlamada zorluk yaşayabilir.
1. **Veriye Erişim ve Kalitesi:** Etkili bir NLP sistemi için büyük ve çeşitli veri setlerine ihtiyaç vardır. Ancak, bu verilere erişim ve veri kalitesi, bazen zorluklar yaratır.

## **Veri Gizliliği ve Etik Konuları:**

1. **Veri Güvenliği ve Gizliliği:** NLP sistemleri genellikle kişisel verileri işler. Bu verilerin güvenliği ve kullanıcıların gizliliği, büyük bir sorumluluk ve zorluk teşkil eder.
1. **Önyargı ve Adil Olmayan Sonuçlar:** Eğitim verilerindeki önyargılar, NLP sistemlerinin adil olmayan veya yanlı sonuçlar üretmesine neden olabilir. Özellikle cinsiyet, ırk ve etnik köken gibi konularda hassasiyet gerektirir.
1. **Şeffaflık ve Hesap Verebilirlik:** NLP sistemlerinin nasıl karar verdiğini anlamak ve bu sistemlerin hesap verebilirliğini sağlamak, karmaşık yapay zeka modellerinde önemli bir meydan okumadır.

# Sonuç

Doğal Dil İşleme (NLP) teknolojileri, modern dünyada sürekli gelişen ve dönüşen bir alan olarak öne çıkmaktadır. Bu teknoloji, insan ve makine arasındaki etkileşimi derinden etkileyerek, bilgiye erişimi kolaylaştırmakta ve günlük hayatımızın birçok yönünü zenginleştirmektedir. NLP'nin uygulama alanları, sosyal medya analizinden sesli asistanlara, makine çevirisinden otomatik metin özetlemeye kadar uzanmakta ve bu süreçte insan yaşamını daha bağlantılı, etkileşimli ve erişilebilir hale getirmektedir.

NLP algoritmaları, dilin karmaşık yapısını anlamak ve işlemek için sürekli geliştirilmekte, bu da makinelerin insan dilini daha iyi anlamasını ve insan gibi doğal bir şekilde yanıt vermesini sağlamaktadır. Bu teknolojinin ilerlemesi, sadece verimliliği ve kolaylığı artırmakla kalmayıp, aynı zamanda kültürlerarası iletişimi destekleyerek dünyayı daha yakın bir hale getirmektedir.

Bu makalenin ele aldığı gibi, NLP'nin etkileri sadece teknolojik ilerlemelerle sınırlı değildir; aynı zamanda sosyal, kültürel ve ekonomik açılardan da derin etkilere sahiptir. NLP'nin geleceği, insan ve makine arasındaki sınırı daha da belirsiz hale getirecek, karmaşık dil işleme görevlerini daha etkin ve doğal hale getirecektir. Kısacası, NLP, yapay zeka ve bilgi teknolojilerinin geleceğinde merkezi bir rol oynamaya devam edecek ve insan hayatını dönüştürmeye devam edecektir.

# Kaynakça

1. Jurafsky, D., & Martin, J. H. (2020). Speech and Language Processing (3rd ed.). Pearson.
2. Stanford NLP. (n.d.). Stanford Named Entity Recognizer (NER) - Example. [https://nlp.stanford.edu/software/CRF-NER.html#Example_Command_Line_Usage](https://nlp.stanford.edu/software/CRF-NER.html#Example_Command_Line_Usage)
3. Natural Language Toolkit (NLTK). (n.d.). Chapter 5: Categorizing and Tagging Words. [https://www.nltk.org/book/ch05.html](https://www.nltk.org/book/ch05.html)
4. Stanford NLP. (n.d.).
5. Hirschberg, J., & Manning, C. D. (2015). Advances in natural language processing. Science, 349(6245), 261-266.
6. Young, S., et al. (2018). Recent trends in deep learning based natural language processing. IEEE Computational Intelligence Magazine, 13(3), 55-75.
7. Nenkova, A., & McKeown, K. (2011). Automatic summarization. Foundations and Trends in Information Retrieval, 5(2–3), 103–233.
8. See, A., et al. (2017). Get to the point: Summarization with pointer-generator networks. Proceedings of the 55th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers).
9. Bao, Y., et al. (2020). Natural language processing in finance: A comprehensive review. Applied Soft Computing, 95, 106384.
10. Loughran, T., & McDonald, B. (2016). Textual analysis in finance. Annual Review of Financial Economics, 8, 289-305.
11. Brown, T. B., et al. (2020). Language models are few-shot learners. arXiv preprint arXiv:2005.14165.
12. Hovy, E., & Yangarber, R. (2020). NLP for the next decade. Proceedings of the 28th International Conference on Computational Linguistics.
13. Hovy, D., & Spruit, S. L. (2016). The social impact of natural language processing. Proceedings of the 54th Annual Meeting of the Association for Computational Linguistics (Volume 2: Short Papers).
14. Sweeney, L., et al. (2017). De-identification of personal information. Journal of Privacy and Confidentiality, 7(1).
