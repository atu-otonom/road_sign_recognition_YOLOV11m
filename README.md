# Yol Levhası Tespiti
Yol levhalarının istikrarlı bir şekilde tespit edilip sınıflandırılması için oluşturulmuş bir repodur. YOLOV11M (Medium) modeli kullanılmış olup, internet üzerinden toplanılan veri setleri ile eğitilmiştir. (Robloflow, kaggle, github, vb.)

Bilgilendirme: Fedora 41 ve Windows 11 üzerinde denenmiş olup eğitimler Fedora 41 tarafında yapılmıştır.

## Kurulum
# Fedora 41 / Windows 11
* Nvidia ekran kartının en güncel sürümüyle birlikte CUDA kurulması gerekmekte.
* Miniconda tarafında env. oluşturulduktan sonra altta verilen pip komutu ile 'pyTorch' framework'ü kurulması gerekmekte. Alttaki terminal komutunun sondaki 'cu126' kısmı CUDA vers. 12.6'yı temsil etmekte, kendi sürümünüze uygun bir şekilde düzeltiniz.
```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu126
```
* pyTorch kurulduktan sonra, env. aktif edip YOLO'nun kurulumunu gerçekleştirmek gerekmekte.
```bash
pip install ultralytics
```
Bilgilendirme: YOLO'nun Nano/Small/Medium versiyonları denenmiş olup alttaki kullanım değerleri elde edilmiştir.
* Nano ≈ (2.5 GB VRAM) 
* Small ≈ (4 GB VRAM)
* Medium ≈ (8 GB VRAM)

## Kullanım
* model.ipynb dosyasını, jupyter notebook ile bağladıktan sonra 'data.yaml' dosyasındaki gerekli pathleri düzelterek ve kendi datasetinizi vererek, her bir cell'i runlayarak modeli oluşturup ya da hali hazırda repo'da bulunan modeli kullanabilirsiniz.
