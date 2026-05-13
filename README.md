# photo-style-transfer

# Demon Slayer Style Transfer

Gerçek manzara fotoğraflarını custom eğitilmiş LoRA + AnyLoRA + ControlNet kullanarak demon slayer (bir ara populer olan bir anime) stiline dönüştüren bir proje.

## Sadece egitilen model test edilir basit adimlari takip ederek hemen calistirilir.
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ismailarslan02/photo-style-transfer-/blob/main/notebooks/demo.ipynb)

## Egitim kodu burdaki link ama karmasik
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ismailarslan02/photo-style-transfer-/blob/main/notebooks/train_and_test_notebook.ipynb)

## Hızlı Başlangıç

Yukarıdaki **"Open in Colab"** butonuna tıklayarak demo notebook'u Colab'da açabilirsiniz.

### Kullanım

1. **"Open in Colab"** butonuna tıklayın
2. Colab'da **Runtime → Change runtime type → T4 GPU** seçin
3. **Runtime → Run all** ile tüm hücreleri çalıştırın
4. Örnek fotoğraf otomatik indirilir, normal bir fotografin anime stili versiyonu üretilir
5. Kendi fotoğrafınızı denemek için ilgili hücrede `USE_EXAMPLE = False` yapın
6. Girilen fotografa gore promptu degistirmeyi unutmayin. --- (ADIM 4 KISMINDA) prompt = "dmnslyr_style, forest, outdoors, best quality" ornek prompt dmnslyr_style kesin olmali stili calistiran asil prompt

**Hiçbir manuel kurulum gerekmemekte** — base model ve LoRA otomatik indirilir.

##  LoRA Eğitim Detayları
- **Base model:** AnyLoRA (Stable Diffusion 1.5)
- **Dataset:** Demon Slayer manzara/sahne görselleri
- **Trigger word:** `dmnslyr_style`
- **Eğitim aracı:** kohya_ss
- **Epoch sayısı:** 10
- **Eğitim ortamı:** Google Colab (T4 GPU)
