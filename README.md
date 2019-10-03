Git Komutları
============

## Translated Versions
- [Versão em português](READMEpt.md)

___

_Sık kullanılan Git komutlarımın listesi_


### Proje Alma ve Oluşturma

| Command | Description |
| ------- | ----------- |
| `git init` | Yerel Git deposunu başlat |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Uzak bir deponun yerel bir kopyasını oluşturun |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Durumu kontrol et |
| `git add [file-name.txt]` | Hazırlama alanına bir dosya ekleyin. |
| `git add -A` | Tüm yeni ve değiştirilmiş dosyaları hazırlama alanına ekle |
| `git commit -m "[commit message]"` | Değişiklikleri kabul et |
| `git rm -r [file-name.txt]` | Bir dosyayı (veya klasörü) kaldırın |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | Dalları listele (yıldız, geçerli dalı gösterir) |
| `git branch -a` | Tüm dalları listele (yerel ve uzak) |
| `git branch [branch name]` | Yeni dal oluştur |
| `git branch -d [branch name]` | Dal sil |
| `git push origin --delete [branch name]` | Uzak bir dalı sil |
| `git checkout -b [branch name]` | Yeni bir şube oluştur ve ona geç |
| `git checkout -b [branch name] origin/[branch name]` | Uzak bir dalı klonla ve ona geç |
| `git branch -m [old branch name] [new branch name]` | Yerel bir dalı yeniden adlandır |
| `git checkout [branch name]` | Bir dala geç |
| `git checkout -` | En son teslim edilen dala geç |
| `git checkout -- [file-name.txt]` | Bir dosyadaki değişiklikleri at |
| `git merge [branch name]` | Bir dalı etkin dalda birleştirme |
| `git merge [source branch] [target branch]` | Bir dalı hedef dalda birleştirme |
| `git stash` | Kirli bir çalışma dizininde saklamak değişiklikleri |
| `git stash clear` | Tüm saklanan girişleri kaldır |

### Projeleri & Paylaşma ve Güncelleme

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Bir dalı uzak havuzunuza itin |
| `git push -u origin [branch name]` | Değişiklikleri uzak havuza doğru itin (ve dalı hatırlayın)) |
| `git push` | Değişiklikleri uzak havuza itin (hatırlanan dal) |
| `git push origin --delete [branch name]` | Uzak bir dalı sil |
| `git pull` | Yerel veri havuzunu en yeni işleme gönder |
| `git pull origin [branch name]` | Uzak havuzdan değişiklikleri çekin |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Uzak bir depo ekle |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Bir havuzun orijin şubesini SSH'ye ayarla |

### Muayene & Karşılaştırma

| Command | Description |
| ------- | ----------- |
| `git log` | Değişiklikleri görüntüle |
| `git log --summary` | Değişiklikleri görüntüle (ayrıntılı) |
| `git diff [source branch] [target branch]` | Birleştirmeden önce değişiklikleri önizle |

