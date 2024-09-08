# Discord Vanity URL Claimer Bot
Bu Python betiği, bir Discord sunucusunda istenen Vanity URL'yi (özel bağlantı) sürekli olarak kontrol eder ve URL kullanılabilir hale geldiğinde onu talep etmeye çalışır. Betik iki farklı token (bir dinleyici ve bir talep edici) kullanarak bu işlemi gerçekleştirir. Dinleyici, mevcut Vanity URL'yi kontrol eder ve talep edici, URL'yi ele geçirmeye çalışır.

# Özellikler
İstenen Vanity URL'yi kontrol eder.
Vanity URL müsait olduğunda, onu talep eder.
Talep işlemi başarısız olursa tekrar denemek üzere çalışmaya devam eder.
Talep işlemi başarılı olduğunda kullanıcıyı bilgilendirir.
Gereksinimler
Bu betiği çalıştırmadan önce aşağıdaki Python kütüphanelerinin kurulu olduğundan emin olun:

pip install requests



# Kullanım
Adımlar
Gerekli Bilgileri Girin: Aşağıdaki sabitleri, kendi bilgilerinizle doldurun:

DESIRED_VANITY_URL: Talep etmek istediğiniz Vanity URL'yi buraya girin.
LISTENER_TOKEN: URL'yi kontrol etmek için kullanılan bot token'ını buraya girin.
STEALER_TOKEN: URL'yi talep etmek için kullanılan bot token'ını buraya girin.
SERVER_ID: Sunucu kimliğini buraya girin.
Dosyayı Kaydedin: Betiği bir Python dosyası olarak (örneğin, vanity_claimer.py) kaydedin.

Çalıştırın: Terminal veya komut satırından şu komut ile çalıştırın:
python vanity_claimer.py


# Örnek
DESIRED_VANITY_URL = "yourdesiredvanityurl"
LISTENER_TOKEN = "yourlistenerbottoken"
STEALER_TOKEN = "yourstealerbottoken"
SERVER_ID = 123456789012345678

# Betik Nasıl Çalışır?
Betik, belirlenen aralıklarla (INTERVAL) Vanity URL'yi kontrol eder.
Eğer Vanity URL istenen URL ile aynıysa, "Vanity URL is already claimed." mesajı verilir.
Eğer URL mevcut değilse, bot URL'yi ele geçirmeye çalışır.
URL ele geçirilirse, "Vanity URL claimed successfully!" mesajı verilir. Aksi takdirde, "Failed to claim desired vanity URL." mesajı iletilir.
Katkıda Bulunma
Herhangi bir hata bildirimi veya iyileştirme önerisi için lütfen bir "issue" açın veya bir "pull request" gönderin.

# Lisans
# Bu proje MIT lisansı ile lisanslanmıştır.
