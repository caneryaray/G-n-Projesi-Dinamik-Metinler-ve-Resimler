<img width="1017" height="913" alt="image" src="https://github.com/user-attachments/assets/47e0dd19-0082-453d-8825-f30d28b92899" /> 

Subject: README.md – Gün Projesi: Dinamik Metinler ve Resimler

# Gün Projesi: Dinamik Metinler ve Resimler

Bu proje, **HTML, CSS ve JavaScript kullanılarak DOM manipülasyonu** konusunu pekiştirmek amacıyla geliştirilmiştir.
Sayfa içeriği JavaScript tarafında tanımlanan bir obje üzerinden **dinamik olarak** güncellenmektedir.

---

## 🎯 Projenin Amacı

* JavaScript ile **DOM elemanlarını seçme**
* `textContent` ve `src` kullanarak **metin ve görsel güncelleme**
* `classList` ile **dinamik class ekleme**
* Obje (object) yapısından gelen verileri sayfaya aktarma
* Statik HTML yerine **veri odaklı** bir yapı kurma mantığını öğrenmek

---

## 🧱 Proje Yapısı

### 🔹 HTML

* Sayfa iskeleti oluşturuldu
* Navbar, içerik alanları ve footer bölümleri tanımlandı
* İçerikler boş bırakılarak JavaScript ile doldurulacak şekilde hazırlandı

### 🔹 CSS

* Sayfa düzeni ve hizalamalar yapıldı
* Menü elemanlarına dinamik olarak `italic` class’ı eklenecek şekilde stil yazıldı
* Genel görünüm sade ve okunabilir tutuldu

### 🔹 JavaScript

* `siteContent` isimli obje içinde tüm metinler ve görseller tanımlandı
* DOM üzerinden seçilen elemanlara bu veriler aktarıldı

---

## ⚙️ Dinamik Olarak Yapılan İşlemler

### 🧭 Navigasyon Menüsü

* Menü linkleri JavaScript ile dolduruldu
* Tüm linklere `italic` class’ı eklendi

```js
navItems[i].textContent = siteContent.nav[`nav-item-${i + 1}`];
navItems[i].classList.add('italic');
```

---

### 🖼️ Orta Görsel

* Sayfadaki ana görsel JavaScript üzerinden dinamik olarak eklendi

```js
document.getElementById('middle-img').src =
  siteContent.images['accent-img'];
```

---

### 📦 Bottom Content Alanı

* Alt kısımdaki başlıklar ve paragraflar obje üzerinden sayfaya aktarıldı
* Doğru sırayla ve doğru alanlara yerleştirildi

---

### 📞 Contact Bölümü

* İletişim başlığı JavaScript ile dinamik olarak güncellendi

```js
document.querySelector('.contact-h4').textContent =
  siteContent.contact['contact-h4'];
```

---

## 🧠 Kazanımlar

Bu proje sayesinde:

* DOM seçiciler (`querySelector`, `querySelectorAll`, `getElementById`)
* Obje içinden veri çekme
* Döngüler ile çoklu eleman yönetimi
* Temiz ve okunabilir JavaScript yazımı
* Frontend projelerde **veri–arayüz ilişkisi**

konularında pratik yapılmıştır.

---

## 🚀 Geliştirilebilir Alanlar

* Responsive tasarım eklenebilir
* İçerikler JSON dosyasından çekilebilir
* Dark / Light tema desteği eklenebilir
* Butonlara etkileşim (event) eklenebilir

---

## 👤 Geliştirici

**Caner Yaray**
Frontend Developer (Junior)
HTML • CSS • JavaScript

---

> Bu proje, frontend geliştirme sürecinde DOM manipülasyonu konusunu öğrenmek ve pekiştirmek amacıyla hazırlanmıştır.

