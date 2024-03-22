# *Özet*
Jupyter Notebook'da bir veri seti kullanarak 3 farklı model eğitimi.
# *Akış*
Önce _Bayesian Optimization_ ile ve veri üzerinde herhnagi bir değişiklik yapmadan bir tahminde bulunduruldu. Daha sonra veri seti normalize edildi ve tekrar _Bayesian Optimization_ kullanarak tahmin yaptırıldı. En son olarak ise normalize edilmiş veri için _Gridsearch_ kullanarak tahmin yaptırıldı.
# *Detaylı Açıklama*
**1. hücre açıklaması**: kütüphanelerin içe aktarılması yapıldı.
**2. hücre açıklaması**: _diabetes.csv_ isimli veri dosyası _pandas_ kütüphanesi yardımıyla okundu, ilk birkaç satır doğrulama amacıyla görüntülendi.
**3. hücre açıklaması**: sadece feature değerlerini kullanmak ve tahmin edilecek olan sonucu çıkarmak için _drop_ metodu kullanıldı.
**4. hücre açıklaması**: _skopt_ paketinden _BayesSearchCV_ metoduyla parametreler rasgele belirlendi.
**5. hücre açıklaması**: _BayesSearchCV_ kütüphanesinden _fit_ metoduyla en iyi parametreler belirlendi ve görüntülendi.
**6. hücre açıklaması**: En iyi parametreler SVC olarak görüntülendi.
**7. hücre açıklaması**: _BayesSearchCV_ kütüphanesinden _predict_ metoduyla tahmin yapıldı ve _sklearn.metrics_ kütüphanesinden _accuracy_score_ ve _confusion_matrix_ metotlarıyla accuracy ve confusion matrix görüntülendi.
**8. hücre açıklaması**: _pandas_ kütüphanesinden _DataFrame_ metoduyla tahmin edilen değerlerin gerçek ve tahmin değerlerini karşılaştıran bir tablo görüntülendi.
**9. hücre açıklaması**: _sklearn.preprocessing_ paketinden _MinMaxScaler_ ve _fit_transform_ metotlarıyla veri normalize edildi.
**10. hücre açıklaması**: normalize edilmiş veri tabloya çevrilip tablo halinde görüntülendi.
**11 hücre açıklaması**: sadece feature değerlerini kullanmak ve tahmin edilecek olan sonucu çıkarmak için _drop_ metodu kullanıldı.
**12. hücre açıklaması**:veri seti _train_test_split_ metodu kullanılarak train ve test gruplarına ayrıldı.
**13. hücre açıklaması**: __GaussianNB_ kütüphanesinden _fit_ ve _predict_ metotları kullanılarak en iyi parametreler belirlendi ve bu parametrelerle tahmin yapıldı.
**14. hücre açıklaması**: _sklearn.metrics_ kütüphanesinden _accuracy_score_ ve _confusion_matrix_ metotlarıyla accuracy ve confusion matrix görüntülendi.
**15. hücre açıklaması**: _pandas_ kütüphanesinden _DataFrame_ metoduyla tahmin edilen değerlerin gerçek ve tahmin değerlerini karşılaştıran tablo görüntülendi.
**16. hücre açıklaması**: sadece feature değerlerini kullanmak ve tahmin edilecek olan sonucu çıkarmak için _drop_ metodu kullanıldı. 
**17. hücre açıklaması**: veri seti _train_test_split_ metodu kullanılarak train ve test gruplarına ayrıldı.
**18. hücre açıklaması**: _GridSearchCV_ kütüphanesinden _param_grid_ attribute ile parametreler rasgele belirlendi.
**19. hücre açıklaması**: _GridSearchCV_ kütüphanesinden _fit_ metoduyla en iyi parametreler belirlendi ve görüntülendi.
**20. hücre açıklaması**: En iyi parametreler SVC olarak görüntülendi.
**21. hücre açıklaması**: _GridSearchCV_ kütüphanesinden _predict_ metoduyla tahmin yapıldı ve _sklearn.metrics_ kütüphanesinden _accuracy_score_ ve _confusion_matrix_ metotlarıyla accuracy ve confusion matrix görüntülendi.
**22. hücre açıklaması**: _pandas_ kütüphanesinden _DataFrame_ metoduyla tahmin edilen değerlerin gerçek ve tahmin değerlerini karşılaştıran tablo görüntülendi.
# *Sonuç*
3 modelin tahminlerindeki karşılaştırmada en fazla accuracy score'a sahip olan modelin veri değiştirilmeden yani normalize edilmeden, _bayesian optimization_ kullanılarak oluşturulan model olduğu görüldü.
