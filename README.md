# Sorting Station - Analog Boyut Ayıklama Sistemi 📦📏

Bu proje, Siemens TIA Portal ve Factory I/O kullanılarak gerçekleştirilmiş, paketleri boyutlarına göre analog sensör verisiyle ayıran bir endüstriyel otomasyon simülasyonudur.

## 🛠 Kullanılan Teknolojiler
- **Yazılım:** TIA Portal V19, Factory I/O
- **PLC:** Siemens S7-1200 (Sanal - PLCSIM)
- **Veri Tipi:** Analog Giriş İşleme (Double Integer - ID30)

## 🚀 Proje Mantığı
Sistem, konveyörden gelen paketlerin yüksekliğini analog sensörle ölçer:
1. **Küçük Paket:** Belirlenen alt eşik değerinin altındaysa 1. hatta yönlendirilir.
2. **Orta Paket:** Belirlenen aralıktaysa 2. hatta yönlendirilir.
3. **Büyük Paket:** Üst eşik değerini aşıyorsa 3. hatta yönlendirilir.

## 📂 Dosya Yapısı ve Kurulum

Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki dosyaları kullanabilirsiniz:

- **TIAV19.zap19**: Siemens TIA Portal V19 için arşivlenmiş PLC projesi. (Açmak için TIA Portal'da `Project > Retrieve` yolunu izleyin.)
- **Proje FactoryIO.factoryio**: Factory I/O simülasyon sahnesi. (Açmak için Factory I/O'da `File > Open` yolunu izleyin.)

### 🛠 Kurulum Adımları
1. PLC projesini TIA Portal ile geri yükleyin (Retrieve).
2. PLCSIM'i başlatın ve kodu sanal PLC'ye yükleyin.
3. Factory I/O sahnesini açın ve `File > Drivers` kısmından S7-PLCSIM'i seçerek 'Connect' butonuna basın.
