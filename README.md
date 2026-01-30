# Waste-Attention-Net

Advanced RealWaste Classification (Attention & DCN)
Bu proje, RealWaste veri setini kullanarak atık türlerini sınıflandırmak için geliştirilmiş, Attention (Dikkat) Mekanizmaları ve Deformable Convolutions (Şekil Değiştirebilen Konvolüsyonlar) ile güçlendirilmiş hibrit bir derin öğrenme mimarisi sunar.

Projenin temel amacı, standart CNN modellerinin ötesine geçerek, şekli bozulmuş veya karmaşık arka plana sahip atık nesnelerinde (ezilmiş şişeler, buruşuk kağıtlar) yüksek sınıflandırma başarısı elde etmektir.

Bu proje, literatürdeki çeşitli tekniklerin özel bir kombinasyonunu içerir:

-Hibrit Veri Zenginleştirme (Mixup & CutMix): Modelin ezberlemesini önlemek ve genelleme yeteneğini artırmak için Mixup ve CutMix tekniklerini olasılıksal olarak birleştiren özel bir collate_fn mekanizması.

-Dinamik Attention Modülleri: ResNet ve EfficientNet mimarilerine entegre edilebilen tak-çıkar (plug-and-play) dikkat blokları:

-CBAM: Hem kanal hem de uzaysal dikkat.

-Coordinate Attention (CA): Konumsal bilgiyi koruyan dikkat mekanizması.

-SimAM: Parametresiz, enerji tabanlı dikkat modülü.

-Deformable Convolutions (DCN): Atık nesnelerinin düzensiz geometrisini (bükülmüş, ezilmiş) daha iyi yakalamak için standart konvolüsyon yerine şekil değiştirebilen katmanlar.

## 📚 Citation

If you use the **RealWaste** dataset or this code in your research, please cite the original paper:

### BibTeX
```bibtex

Single, S., Iranmanesh, S., & Raad, R. (2023). RealWaste: A Novel Real-Life Data Set for Landfill Waste Classification Using Deep Learning. Information, 14(12), 633. https://doi.org/10.3390/info14120633

URL:https://archive.ics.uci.edu/dataset/908/realwaste
