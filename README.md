# 🚀 BlackPulse v3.0 - Advanced Network Performance Testing Tool

<div align="center">

```
██████╗ ██╗      █████╗  ██████╗██╗  ██╗██████╗ ██╗   ██╗██╗     ███████╗███████╗
██╔══██╗██║     ██╔══██╗██╔════╝██║ ██╔╝██╔══██╗██║   ██║██║     ██╔════╝██╔════╝
██████╔╝██║     ███████║██║     █████╔╝ ██████╔╝██║   ██║██║     ███████╗█████╗  
██╔══██╗██║     ██╔══██║██║     ██╔═██╗ ██╔═══╝ ██║   ██║██║     ╚════██║██╔══╝  
██████╔╝███████╗██║  ██║╚██████╗██║  ██╗██║     ╚██████╔╝███████╗███████║███████╗
╚═════╝ ╚══════╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚═╝      ╚═════╝ ╚══════╝╚══════╝╚══════╝
```

**Professional Grade Network Performance Testing Suite**

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/license-Educational%20Use-red.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20Termux-green.svg)](README.md)
[![Version](https://img.shields.io/badge/version-3.0-brightgreen.svg)](README.md)

</div>

## 📋 İçindekiler

- [🎯 Genel Bakış](#-genel-bakış)
- [✨ Özellikler](#-özellikler)
- [🔧 Kurulum](#-kurulum)
- [🚀 Kullanım](#-kullanım)
- [📊 Test Modları](#-test-modları)
- [⚙️ Konfigürasyon](#️-konfigürasyon)
- [📈 Raporlama](#-raporlama)
- [🛡️ Güvenlik ve Yasal Uyarı](#️-güvenlik-ve-yasal-uyarı)
- [🤝 Katkıda Bulunma](#-katkıda-bulunma)
- [📄 Lisans](#-lisans)

## 🎯 Genel Bakış

**BlackPulse v3.0**, ağ performansı ve güvenlik testleri için geliştirilmiş profesyonel düzeyde bir araçtır. Çoklu protokol desteği, gerçek zamanlı analitik ve gelişmiş raporlama özellikleri ile ağ altyapınızın performansını ve dayanıklılığını test etmenizi sağlar.

### 👨‍💻 Geliştirici
**Muhammed Cengiz** tarafından geliştirilmiştir.

### 🎓 Amaç
Bu araç **eğitim ve test amaçlı** olarak yazılmıştır. Ağ güvenliği öğreniminde ve kendi sistemlerinizin performans testlerinde kullanılması için tasarlanmıştır.

## ✨ Özellikler

### 🌐 Çoklu Protokol Desteği
- **TCP Flood Test** - Yüksek performanslı TCP bağlantı testi
- **HTTP/HTTPS Flood** - Web sunucu performans testi
- **UDP Flood** - UDP paket bombardımanı testi
- **WebSocket Test** - WebSocket protokol testi
- **DNS Flood** - DNS çözümleme stres testi
- **ICMP Ping Test** - ICMP ping flood testi

### 📊 Gelişmiş Analitik
- Gerçek zamanlı performans izleme
- Detaylı latency analizi ve percentile hesaplamaları
- Bağlantı başarı/başarısızlık oranları
- Sistem kaynak kullanım takibi
- Bandwidth ve RPS (Request Per Second) metrikleri

### 🎨 Profesyonel Arayüz
- Renkli ve kullanıcı dostu terminal arayüzü
- İnteraktif menü sistemi
- Gerçek zamanlı progress bar
- Detaylı hata raporlama

### 📈 Kapsamlı Raporlama
- JSON formatında detaylı raporlar
- CSV formatında veri dışa aktarımı
- Grafik raporları (matplotlib ile)
- Konsol tabanlı özet raporlar

## 🔧 Kurulum

### 📋 Sistem Gereksinimleri

- **Python 3.8+**
- **Linux** veya **Termux** (Android)
- Minimum 2GB RAM
- İnternet bağlantısı (bağımlılık kurulumu için)

### 🐧 Linux Kurulumu

```bash
# Depoyu klonlayın
git clone https://github.com/Muhammedcengizz598/blackpulse.git
cd blackpulse

# Alternatif olarak manuel kurulum
pip3 install dnspython requests aiohttp psutil pyyaml matplotlib numpy tabulate websockets scapy
```

### 📱 Termux Kurulumu

```bash
# Termux paketlerini güncelleyin
pkg update && pkg upgrade

# Python ve gerekli araçları kurun
pkg install python git

# Depoyu klonlayın
git clone https://github.com/Muhammedcengizz598/blackpulse.git
cd blackpulse

pip3 install dnspython requests aiohttp psutil pyyaml matplotlib numpy tabulate websockets scapy


```

### 📦 Gerekli Bağımlılıklar

#### Zorunlu Bağımlılıklar:
```
dnspython>=2.0.0
requests>=2.25.0
aiohttp>=3.8.0
psutil>=5.8.0
pyyaml>=6.0
```

#### Opsiyonel Bağımlılıklar (Gelişmiş Özellikler):
```
matplotlib>=3.5.0
numpy>=1.21.0
tabulate>=0.9.0
websockets>=10.0
scapy>=2.4.5
```

## 🚀 Kullanım

### 🎮 İnteraktif Mod

```bash
# Programı başlatın
python3 black_pulse.py

# Menüden istediğiniz test modunu seçin
# Hedef IP/domain ve parametreleri girin
# Testi başlatın
```

### ⚡ Komut Satırı Modu

```bash
# Hızlı test
python3 black_pulse.py --target example.com --port 80 --mode HTTP_FLOOD --threads 50 --duration 60

# Konfigürasyon dosyası ile
python3 black_pulse.py --config test_config.yaml

# Sessiz mod (sadece sonuçlar)
python3 black_pulse.py --target 192.168.1.1 --quiet
```

### 📝 Konfigürasyon Dosyası Oluşturma

```bash
# Örnek konfigürasyon dosyası oluştur
python3 black_pulse.py --create-config
```

## 📊 Test Modları

### 1. 🔗 TCP Flood Test
Hedef sunucuya yüksek sayıda TCP bağlantısı açarak performans testi yapar.

```python
# Örnek kullanım
Mode: TCP_FLOOD
Target: 192.168.1.100:80
Threads: 100
Duration: 120 seconds
```

### 2. 🌐 HTTP/HTTPS Flood Test
Web sunucularının HTTP/HTTPS isteklerine karşı dayanıklılığını test eder.

```python
# HTTP Test
Mode: HTTP_FLOOD
Target: http://example.com
Threads: 50
Duration: 60 seconds

# HTTPS Test
Mode: HTTPS_FLOOD
Target: https://secure.example.com
Threads: 30
Duration: 90 seconds
```

### 3. 📡 UDP Flood Test
UDP protokolü üzerinden paket bombardımanı gerçekleştirir.

```python
Mode: UDP_FLOOD
Target: 192.168.1.100:53
Packet Size: 1024 bytes
Threads: 200
```

### 4. 🔄 WebSocket Test
WebSocket bağlantılarının performansını ve kararlılığını test eder.

```python
Mode: WEBSOCKET_TEST
Target: ws://example.com:8080
Concurrent Connections: 50
Duration: 120 seconds
```

### 5. 🌍 DNS Flood Test
DNS sunucularının sorgu işleme kapasitesini test eder.

```python
Mode: DNS_FLOOD
Target Domain: example.com
DNS Servers: 8.8.8.8, 1.1.1.1
Threads: 100
```

### 6. 📶 ICMP Ping Test
ICMP ping paketleri ile ağ gecikmesi ve paket kaybı testi yapar.

```python
Mode: ICMP_PING
Target: 192.168.1.1
Packet Size: 64 bytes
Interval: 0.1 seconds
# Not: Root yetkileri gerektirir
```

## ⚙️ Konfigürasyon

### 📄 YAML Konfigürasyon Örneği

```yaml
target:
  ip: "192.168.1.100"
  port: 80
  domain: "example.com"

test:
  mode: "HTTP_FLOOD"
  threads: 100
  duration: 120
  timeout: 5

advanced:
  send_data: true
  data_size: 1024
  wait_response: false
  socket_pool_size: 10

output:
  json_report: true
  csv_report: true
  graph_report: true
  console_report: true
```

### 🔧 Gelişmiş Parametreler

| Parametre | Açıklama | Varsayılan | Aralık |
|-----------|----------|------------|--------|
| `threads` | Eşzamanlı thread sayısı | 100 | 1-2000 |
| `duration` | Test süresi (saniye) | 120 | 1-7200 |
| `timeout` | Bağlantı timeout (saniye) | 5 | 0.1-60 |
| `data_size` | Gönderilecek veri boyutu | 1024 | 1-65536 |
| `socket_pool_size` | Socket havuzu boyutu | 10 | 1-100 |

## 📈 Raporlama

### 📊 Konsol Raporu
Test sonrasında detaylı konsol raporu görüntülenir:
- Test özeti ve parametreler
- Performans metrikleri (RPS, başarı oranı)
- Latency analizi (ortalama, medyan, percentile)
- Hata analizi ve dağılımı
- Sistem kaynak kullanımı
- Optimizasyon önerileri

### 📄 JSON Raporu
Programatik erişim için JSON formatında detaylı rapor:
```json
{
  "metadata": {
    "version": "3.0",
    "generated_at": "2024-01-15T10:30:00",
    "duration_seconds": 120
  },
  "metrics": {
    "requests": {
      "total": 15000,
      "successful": 14500,
      "failed": 500,
      "success_rate_percent": 96.67
    },
    "performance": {
      "average_rps": 125.5,
      "max_concurrent_connections": 100
    }
  }
}
```

### 📊 Grafik Raporları
Matplotlib ile görsel raporlar:
- Latency değişim grafiği
- Latency dağılım histogramı
- Response size değişimi
- Başarı/başarısızlık pasta grafiği

### 📋 CSV Dışa Aktarım
Veri analizi için CSV formatında:
```csv
Timestamp,Latency_ms,Response_Size,Success
1642248600.123,45.2,1024,1
1642248600.234,52.1,1024,1
```

## 🛡️ Güvenlik ve Yasal Uyarı

### ⚠️ ÖNEMLİ UYARI

Bu araç **yalnızca eğitim ve test amaçlı** geliştirilmiştir. Kullanırken aşağıdaki kurallara uymanız zorunludur:

### ✅ İzin Verilen Kullanımlar
- **Kendi sistemlerinizde** performans testi
- **Eğitim amaçlı** ağ güvenliği öğrenimi
- **Yetkili olduğunuz** sistemlerde penetrasyon testi
- **Laboratuvar ortamında** araştırma ve geliştirme

### ❌ Yasak Kullanımlar
- Başkalarının sistemlerine **izinsiz erişim**
- **DDoS saldırıları** gerçekleştirme
- **Hizmet kesintisine** neden olma
- **Yasal olmayan** ağ faaliyetleri

### 🔒 Sorumluluk Reddi

- Bu aracın **yanlış kullanımından** geliştiriciler sorumlu tutulamaz
- Kullanıcı, aracı **kendi sorumluluğunda** kullanır
- **Yasal yükümlülükler** kullanıcıya aittir
- Araç **sadece test ve eğitim** amaçlıdır

### 📜 Etik Kullanım İlkeleri

1. **İzin Alın**: Test edeceğiniz sistemler için gerekli izinleri alın
2. **Zarar Vermeyin**: Sistemlere kalıcı zarar vermekten kaçının
3. **Öğrenin**: Aracı güvenlik bilginizi artırmak için kullanın
4. **Paylaşın**: Öğrendiklerinizi etik çerçevede paylaşın

## 🔧 Sistem Optimizasyonu

### 🐧 Linux Optimizasyonu

```bash
# Dosya descriptor limitini artırın
ulimit -n 65536

# TCP ayarlarını optimize edin
echo 'net.core.somaxconn = 65535' >> /etc/sysctl.conf
echo 'net.ipv4.tcp_max_syn_backlog = 65535' >> /etc/sysctl.conf
sysctl -p

# Performans için CPU governor ayarı
echo performance > /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
```

### 📱 Termux Optimizasyonu

```bash
# Termux için özel ayarlar
termux-wake-lock  # Uyku modunu engelle
termux-battery-status  # Batarya durumunu kontrol et

# Bellek optimizasyonu
export PYTHONOPTIMIZE=1
export PYTHONDONTWRITEBYTECODE=1
```

## 🤝 Katkıda Bulunma

### 🛠️ Geliştirme Ortamı

```bash
# Geliştirme için depoyu fork edin
git clone https://github.com/Muhammedcengizz598/blackpulse.git
cd blackpulse

# Geliştirme bağımlılıklarını kurun
pip install -r requirements-dev.txt

# Test ortamını kurun
python -m pytest tests/
```

### 📝 Katkı Süreci

1. **Fork** edin ve **branch** oluşturun
2. **Değişikliklerinizi** yapın
3. **Test** edin ve **dokümante** edin
4. **Pull Request** gönderin

### 🐛 Hata Bildirimi

Hata bulduğunuzda lütfen aşağıdaki bilgileri ekleyin:
- İşletim sistemi ve versiyonu
- Python versiyonu
- Hata mesajı ve stack trace
- Yeniden üretme adımları

## 📞 İletişim ve Destek

### 📧 İletişim
- **Geliştirici**: Muhammed Cengiz
- **E-posta**: [cengizmuhammed598@gmail.com]

## 📄 Lisans

Bu proje **MİT** lisansı altında dağıtılmaktadır.

### 📋 Lisans Koşulları

- ✅ **Eğitim amaçlı** kullanım serbest
- ✅ **Kişisel test** ortamlarında kullanım
- ✅ **Kaynak kodu** inceleme ve öğrenme
- ❌ **Ticari kullanım** yasak
- ❌ **Kötü amaçlı** kullanım yasak
- ❌ **Yeniden dağıtım** kısıtlı

## 🔄 Sürüm Geçmişi

### v3.0 (Mevcut)
- 🆕 Çoklu protokol desteği
- 🆕 Gerçek zamanlı analitik
- 🆕 Grafik raporlama
- 🆕 Konfigürasyon dosyası desteği
- 🆕 Gelişmiş hata yönetimi

### v2.x
- TCP ve HTTP temel testler
- Basit konsol çıktısı

### v1.x
- İlk sürüm
- Temel TCP testi

## 🙏 Teşekkürler

Bu projenin geliştirilmesinde katkıda bulunan herkese teşekkürler:

- **Açık kaynak topluluğu** - Kullanılan kütüphaneler için
- **Güvenlik araştırmacıları** - İlham ve geri bildirimler için
- **Beta test kullanıcıları** - Hata raporları ve öneriler için

---

<div align="center">

**⚠️ Bu araç sadece eğitim ve test amaçlıdır. Etik ve yasal kurallara uygun kullanın! ⚠️**

**Made with ❤️ by Muhammed Cengiz**

</div>
