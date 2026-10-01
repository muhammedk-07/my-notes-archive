# 🛠️ Git Temel Komutlar Rehberi

Bu rehber, Git kullanırken en sık ihtiyaç duyacağınız temel komutları ve işlevlerini içerir.

## 🚀 1. Çalışma Alanı Oluşturma (Starting a Working Area)

_Projenizi başlatmak veya var olan bir projeyi yerel bilgisayarınıza indirmek için kullanılır._

- **`git init`**
  - **Açıklama:** Boş bir Git deposu (repository) oluşturur veya var olan bir depoyu yeniden başlatır. Projenizin ilk adımında kullanılır.
- **`git clone`**
  - **Açıklama:** Uzak sunucudaki (GitHub, GitLab vb.) mevcut bir depoyu bilgisayarınızdaki yeni bir dizine kopyalar.

## 📝 2. Değişiklikler Üzerinde Çalışma (Working on the Current Change)

_Dosyalar eklemek, silmek, taşımak veya yapılan değişiklikleri geri almak için kullanılır._

- **`git add`**
  - **Açıklama:** Dosya içeriklerini dizine (sahneye/staging area) ekler. Commit öncesi hazırlık aşamasıdır.
- **`git mv`**
  - **Açıklama:** Bir dosyayı, dizini veya sembolik bağı taşır ya da adını değiştirir.
- **`git rm`**
  - **Açıklama:** Dosyaları hem çalışma dizininden (working tree) hem de Git dizininden kaldırır.
- **`git restore`**
  - **Açıklama:** Çalışma dizinindeki dosyaları eski durumuna getirir, yapılan değişiklikleri geri alır.

## 🔍 3. Geçmişi ve Durumu İnceleme (Examining History and State)

_Projenizin anlık durumunu görmek ve geçmişte yapılanları incelemek için kullanılır._

- **`git status`**
  - **Açıklama:** Çalışma dizininin ve sahnenin (staging area) anlık durumunu gösterir (Hangi dosyalar değişti, hangileri takibe alınmadı vb.).
- **`git diff`**
  - **Açıklama:** Commit'ler arasındaki, commit ile çalışma dizini arasındaki veya dosyalar arasındaki değişiklikleri gösterir.
- **`git log`**
  - **Açıklama:** Projedeki commit (işleme) geçmişini kronolojik olarak listeler.
- **`git show`**
  - **Açıklama:** Belirli Git nesnelerinin (commit, tag vb.) detaylı içeriğini gösterir.
- **`git grep`**
  - **Açıklama:** Belirli bir kalıba/kelimeye uyan satırları proje dosyaları içinde arar ve yazdırır.
- **`git bisect`**
  - **Açıklama:** İkili arama (binary search) algoritmasını kullanarak projeye hata (bug) getiren commit'i tespit etmenizi sağlar.

## 🌱 4. Geçmişi Büyütmek, İşaretlemek ve Şekillendirmek (Grow, Mark and Tweak History)

_Dallanmalar (branch) oluşturmak, değişiklikleri kaydetmek ve geçmişi düzenlemek için kullanılır._

- **`git branch`**
  - **Açıklama:** Dalları (branch) listeler, yeni dal oluşturur veya mevcut dalları siler.
- **`git switch`**
  - **Açıklama:** Çalıştığınız dallar (branch) arasında geçiş yapmayı sağlar.
- **`git commit`**
  - **Açıklama:** Sahneye eklenen (staged) değişiklikleri depoya kalıcı olarak kaydeder.
- **`git merge`**
  - **Açıklama:** İki veya daha fazla geliştirme geçmişini (farklı dalları) birleştirir.
- **`git rebase`**
  - **Açıklama:** Bir daldaki commit'leri, başka bir dalın ucunun (base tip) üzerine yeniden uygular; temiz bir geçmiş sağlar.
- **`git reset`**
  - **Açıklama:** `HEAD` konumunu veya dizini belirli bir duruma/commit'e sıfırlar.
- **`git tag`**
  - **Açıklama:** Belirli commit'lere etiket (sürüm numaraları gibi: v1.0.0) ekler, listeler veya siler.
- **`git backfill`**
  - **Açıklama:** Kısmi klonlanmış (partial clone) bir depoda eksik olan nesneleri indirir.
- **`git history`**
  - **Açıklama:** _(Deneysel)_ Git geçmişini yeniden yazmak/düzenlemek için kullanılır.

## 🤝 5. İş Birliği Yapma (Collaborate)

_Ekip arkadaşlarınızla veya uzak sunucularla (remote) senkronize olmak için kullanılır._

- **`git fetch`**
  - **Açıklama:** Uzak bir depodaki nesneleri ve referansları yerel bilgisayarınıza indirir (ancak mevcut kodunuzla birleştirmez).
- **`git pull`**
  - **Açıklama:** Uzak depodaki değişiklikleri indirir (`fetch`) ve doğrudan mevcut yerel dalınızla birleştirir (`merge`).
- **`git push`**
  - **Açıklama:** Yerel depoda yaptığınız commit'leri ve ilişkili nesneleri uzak sunucuya gönderip günceller.
  ## Kolaylaştırıcı Komutlar
- **`find . \( -name "*.c" -o -name "*.h" \) ! -path "./Hedef_Klasor/*" -exec cp {} "./Hedef_Klasor/" \;`**
  - **Açıklama:** Bu yapı bir klasör altındaki tüm seçili uzantılı dosyaları hedef klasöre taşımak için kullanılır.
