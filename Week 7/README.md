# CODIMIS 
## Javascript Eğitimi Yedinci Hafta Soruları
1 - "Working directory" bilgisayarımızdaki git reposuna verilen isimdir.

* A) Doğru
* B) Yanlış

2 - "Staging Area/Staging Index" commit işlemi yapıldıktan dosyaların geçtiği alandır.

* A) Doğru
* B) Yanlış

3 - Aşağıdakilerden hangisi bir git reposu oluşturulmak için kullanılır?

* A) Git start
* B) Git create
* C) Git init
* D) Git clone

4 - Aşağıdakilerden hangisi bir git reposunda değişiklik yapılmış ancak kaydedilmemiş dosyaları görüntülemek için kullanılır?

* A) Git status
* B) Git log
* C) Git init
* D) Git clone

5 - "5275ad" ile başlayan SHA koduna sahip commit kim tarafından atılmıştır?

```
commit c9bfd49f052f749dd61d276efeb56aec07e3dda4
Author: Tas, Ugur <ugur@test.com>
Date:   Sun Apr 18 22:53:58 2021 +0200

    questions for week 6 are created and new questions are added to week 1

commit 5275adc96da53926f786234aa4cbc042ac930996
Author: Caner Ünal <caner@test.com>
Date:   Sun Apr 11 22:29:04 2021 +0300

    Week 1 new question added

commit 078d2345e90aafcdff5495491784ced378c7bc18
Merge: ca61274 a33a901
Author: Tas, Ugur <ugur@test.com>
Date:   Sun Apr 11 21:24:52 2021 +0200

    merge

commit ca6127414ddd24f59935f95967f1214042b69165
Author: Tas, Ugur <ugur@test.com>
Date:   Sun Apr 11 21:18:25 2021 +0200

    Questions for week 5
```

* A) Uğur TAŞ
* B) Caner Ünal
* C) Rahmetli Başkan Kennedy
* D) Taçsız Kral Pele

6 - Hangi tuş git log ekranını kapatmak için kullanılır?

* A) K
* B) J
* C) Q
* D) B

7 - Hangi git komutu commitlerde yapılan değişiklikleri gösterir?

* A) git log
* B) git log --oneline
* C) git log --stat
* D) git log --patch

8 - Hangi git komutu commitlerde ne kadar değişiklik yapıldığını gösterir?

* A) git log
* B) git log --oneline
* C) git log --stat
* D) git log --patch

9 - git show ve git log -p komutları arasındaki fark hangisidir?

* A) git show ve git log -p arasında fark yoktur
* B) git show tek commit gösterirken git log -p tüm commitler için sonuç gösterir
* C) git show sadece commitleri gösterirken git log -p commitlerdeki değişiklikleri gösterir
* D) git show projedeki branchleri gösterirken git log -p commitlerdeki değişiklikleri gösterir

10 - Değişiklik yapılan tüm dosyaları bulunduğum klasörden bağımsız olarak staging indexe eklemek için hangi komut kullanılır?

* A) git add
* B) git add .
* C) git add -A
* D) git add all

11 - Yapılmış ama commitlenmemiş değişiklikleri görmek için hangi komut kullanılır?

* A) git show
* B) git log
* C) git status
* D) git diff

12 - Gitignore dosyası ne işe yarar?

* A) Yapılan değişiklikleri görmek için kullanılır
* B) Git commit mesajlarını tutmak için kullanılır
* C) Takip edilmesinin istenmediğinde dosyaları tutmak için kullanılır 
* D) Git üzerindeki değişiklikleri saklamak için kullanılır.

13 - Git loglarında tag bilgisinin de gösterilmesi için hangi parametrenin kullanılması gerekiyor?

* A) --show-tags
* B) --tags
* C) --display-all
* D) --decorate

14 - Git branchlerini listelemek için hangi komut kullanılır?

* A) git show
* B) git log
* C) git branch
* D) git branch list

15 - "git branch codimis" ve "git branch -d codimis" arasında ne fark vardır? 

* A) İkinci komut branch yoksa oluşturur
* B) ilk komut oluştururken ikincisi siler
* C) İkinci komut commit atarak oluşturur
* D) İlk komut o branche geçmeyi sağlar

16 - Aşağıdaki git revert kullanımı ile hangi işlemi yapmış oluruz?
```
caner.unal@CANERUNAL Javascript-quiz-questions (main)
git revert aa41fa7
[main 96fd8ff] Revert "Week 3 changed"

1 file changed, 1 insertion (+), 1 deletion (-)
```

* A) aa41fa7 id li commit silinir
* B) aa41fa7 id li commit teki değişiklikleri geri alınıp, yeni bir commit atılır
* C) Değişiklikleri repository den kaldırıp kendi localimize ekler
* D) aa41fa7 id li commit ten sonraki tüm değişiklikleri siler ve bu id li commit e geri döner