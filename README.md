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

@Article{info14120633,
AUTHOR = {Single, Sam and Iranmanesh, Saeid and Raad, Raad},
TITLE = {RealWaste: A Novel Real-Life Data Set for Landfill Waste Classification Using Deep Learning},
JOURNAL = {Information},
VOLUME = {14},
YEAR = {2023},
NUMBER = {12},
ARTICLE-NUMBER = {633},
URL = {https://www.mdpi.com/2078-2489/14/12/633},
ISSN = {2078-2489},
DOI = {10.3390/info14120633}
}
