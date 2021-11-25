# Git

# Git

## Git initialization

Let's Learn Git
When creating a website, chances are, you will collaborate with other people.
Git is a tool that makes it easy for you to develop and collaborate with your team.
Let's learn Git together.
(It is recommended that you study the Command Line before this lesson. Link...)

You and your friends will create a website together.
While you are just trying team development for the first time, your friends are already experts. Let's learn Git while following their team's development experience.

Maybe you often think "I've never done team development before. Where should I start?" so here we will learn how to use git for team development.

Git is operated from the terminal.
First, to get started, you need to run the git init command.

```git
$ git init
```

You don't need to type $ which appears in the terminal.

## Adding Files to Share

There are 3 steps to team development.
1. Make changes to the file
2. Preparing to share change
3. Share changes

Look at steps 2 & 3. You need to share the code you have written with others to do team development. That's what Git is for.

Suppose here you just created an index.html file! So, how can you share it?

First, you need to select the files you want to share via git.
To select a file, use the command git add file_name.

```git
$ git add index.html
```

Before we could share files. We will save the selected files with a message. Then we are ready to share it.

To record the selected files, run the command git commit -m "message"
We call this kind of save a commit. Please remember, yes.

The message should describe the content you want to commit.
By the way, this message is called a commit message and usually this message will be made in English to make it easier to work with international teams.

```git
$ git commit -m "create index.html"
```
With git add and git commit, the 2 commands we studied, you're ready to share files.

## Added Remote Repository

Git uses something called a remote (or remote repository) to store shared files.
Developers share files by uploading to and downloading from remote.

You need a remote URL to upload. This is the remote URL I prepared this time https://github.com/EndyPratama/Git.git

When you add a remote, you will need a name. Usually, developers use the origin name.
More specifically, to register a remote, type git remote add origin remote_name URL, as in the image on the right.

```git
git remote add origin https://github.com/EndyPratama/Git.git
```

## Uploading Files

OK, now let's try uploading a file to the remote! We can upload to the remote we created earlier by running: git push origin master
Uploading like this with Git is called push.

```git
$ git push origin master
```

## Downloading Files

It's good that you have completed the data push, now your friends can download the file by running git pull origin master
Downloading a file like this is called a pull. You have to remember it.

```git
$ git pull origin master
```

## Reviewing Git Flow

Okay, now you and your friends can work together to complete a project.
Now, let's review what we've learned so far. With these 4 commands
1. git add
2. git commit
3. git push
4. git pull

we can already share files with each other.
Learning Git doesn't end here, there are many others, let's learn together..

## Git Status

In team development, it is important to recognize the changes you are making and choose what changes to share with your team. It will be a problem if you share incomplete code by accident. Therefore, let's learn how to recognize and choose the code that we share.

First, it's important to recognize the changes you've made. Using git status, you can display a list of files that have been modified.
Usually files that have been modified will be red. While the files that have been added (add) are green.

```git
$ git status
```

## Git Diff

git status is really useful. Then can we see the content change too? Of course we can, with the git diff command we can see the content changes

```git
$ git diff
```

The code that has been deleted or replaced will be red while the new code will turn green.

## Commit Message

When writing commits you should write a descriptive commit message so that if someone sees it, they can easily understand what changes have been made.
Suppose in your stylesheet you change the color. Then a good commit like this.
```git
$ git commit -m "Change subtitle color"
```

## Git Log

Earlier you said I had to write commit messages that other people could easily understand, but how can they be seen?

Good question, again!
Using the git log command, you or someone else can see the commits.

With git log, can I see both the commit message and the changes made?

To see the changes, you can use git log -p.
With the up and down arrows, you can scroll through the changes. To exit, simply press the Q key.

[Indonesia]
## Inisialisasi Git

Mari Mempelajari Git
Saat membuat website, Kemungkinan besar, kalian akan berkolaborasi dengan orang lain.
Git adalah tool yang memudahkan kalian untuk melakukan pengembangan dan berkolaborasi dengan tim.
Mari kita mempelajari Git bersama.
(Kalian direkomendasikan untuk memperlajari Command Line sebelum pelajaran ini. Link ...)

Kalian dan teman kalian akan membuat website bersama-sama.
Sementara kalian baru pertama kali mencoba pengembangan tim, sedangkan teman kalian sudah ahli. Mari mempelajari Git sambil mengikuti pengalaman pengembangan tim mereka.

Mungkin kalian sering berpikir "Aku belum pernah melakukan pengembangan tim sebelumnya. Dari mana aku harus memulai?" maka disini kita akan belajar cara menggunakan git untuk pengembangan tim.

Git dioperasikan dari terminal.
Pertama, untuk memulai, kalian perlu untuk menjalankan command git init.

```git
$ git init
```

Kamu tidak perlu untuk mengetik $ yang muncul pada terminal.

## Menambahkan File untuk Dibagikan

Ada 3 langkah pada pengembangan tim.
1. Buat perubahan ke file
2. Persiapan untuk membagikan perubahan
3. Bagikan perubahan

Lihat pada step 2 & 3. Kaluan perlu untuk membagikan code yang telah kalian tulis dengan orang lain untuk melakukan pengembangan tim. Itu gunanya Git.

Misalkan disini kalian baru membuat file index.html! Jadi, bagaimana kalian bisa membagikannya?

Pertama, kalian perlu memilih file-file yang ingin kalian bagikan lewat git.
Untuk memilih sebuah file, gunakan command git add file_name.

```git
$ git add index.html
```

Sebelum kita bisa berbagi file. Kita akan simpan file-file yang dipilih dengan pesan. Lalu kita siap untuk membagikannya.

Untuk merekam file yang dipilih, jalankan command git commit -m "pesan"
Kita menyebut penyimpanan seperti ini sebagai commit. Mohon diingat, ya.

Pesan tersebut seharusnya mendeskripsikan konten yang mau di commit.
Ngomong-ngomong, pesan ini disebut pesan commit dan biasanya pesan ini akan di buat dalam bahasa Inggris untuk mempermudah kerja sama dengan tim internasional.

```git
$ git commit -m "create index.html"
```
Dengan git add dan git commit, 2 command yang sudah kita pelajari, kalian sudah siap untuk berbagi file.

## Menambahkan Remote Repository

Git menggunakan sesuatu yang disebut remote (atau remote repository) untuk menyimpan file-file yang dibagikan.
Pengembang membagikan file dengan mengunggah ke dan mengunduh dari remote.

Kamu perlu URL remote untuk mengunggah. Ini adalah URL remote yang aku siapkan kali ini https://github.com/EndyPratama/Git.git

Saat kamu menambahkan remote, kamu akan memerlukan nama. Biasanya, pengembang menggunakan nama origin.
Lebih spesifik, untuk mendaftarkan remote, ketik git remote add origin remote_name URL, seperti pada gambar di kanan.

```git
git remote add origin https://github.com/EndyPratama/Git.git
```

## Mengunggah File

Oke, sekarang mari coba mengunggah sebuah file ke remote! Kita dapat mengunggah ke remote yang kita buat sebelumnya dengan menjalankan: git push origin master 
Mengunggah seperti ini dengan Git disebut push.

```git 
$ git push origin master
```

## Mengunduh File

Bagus kalian telah menyelesaikan push data, sekarang teman kalian dapat mengunduh file dengan menjalankan git pull origin master
Mengunduh file seperti ini disebut pull. Kamu harus mengingatnya.

```git 
$ git pull origin master
```

## Meninjau Alur Git

Oke sekarang kalian dan teman kalian sudah bisa bekerja sama dalam menyelesaikan suatu projek. 
Sekarang, mari kita meninjau ulang apa yang sudah kita pelajari sejauh ini. Dengan 4 command ini
1. git add
2. git commit
3. git push
4. git pull

kita sudah dapat berbagi file satu sama lain. 
Belajar Git tidak sampai sini saja, masih ada banyak yang lain, yuk belajar bersama..

## Git Status

Dalam pengembangan tim, penting untuk mengenali perubahan-perubahan yang kalian buat dan memilih perubahan apa yang harus kalian bagikan dengan timmu. Akan jadi masalah jika kalian membagikan code yang tidak komplit tanpa disengaja. Maka dari itu mari kita belajar bagaimana mengenali dan memilih code yang kita bagikan.

Pertama, penting untuk mengenali perubahan-perubahan yang sudah kalian lakukan. Dengan menggunakan git status, kalian dapat menampilkan daftar file-file yang sudah dimodifikasi.
Biasanya file yang telah dimodifikasi akan berwarna merah. Sedangkan file - file yang telah ditambahkan (add) berwarna hijau.

```git
$ git status
```

## Git Diff

git status benar-benar berguna. Lalu bisakah kita melihat perubahan kontennya juga? Tentu bisa, dengan command git diff kita dapat melihat perubahan konten

```git
$ git diff
```

code yang telah dihapus atau diganti akan berwarna merah sedanakan code yang baru akan berubah menjadi warna hijau.

## Pesan Commit

Dalam penulisan commit kalian harus menulis pesan commit yang deskriptif sehingga jika seseorang melihatnya, mereka bisa mengerti dengan mudah perubahan apa yang sudah dibuat.
Misalkan dalam stylesheet kalian merubah warna. Maka commit yang baik seperti ini.
```git
$ git commit -m "Change subtitle color"
```

##  Git Log

Sebelumnya kamu bilang aku harus menulis pesan commit yang bisa dimengerti dengan mudah oleh orang lain, tapi bagaimana mereka bisa terlihat?

Pertanyaan bagus, sekali lagi!
Dengan menggunakan command git log, kamu atau orang lain dapat melihat commit-commit.

Dengan git log, bisakah aku melihat kedua pesan commit dan perubahan-perubahan yang dibuat?

Untuk melihat perubahan-perubahan, kamu bisa menggunakan git log -p.
Dengan panah atas dan bawah, kamu dapat bergulir ke seluruh perubahan. Untuk keluar, cukup tekan tombol Q.
