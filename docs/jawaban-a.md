>Tubagus A Fauzan M_10323050
* Analisis Kondisi  
  Jelas ini aman, sudah diisi formnya
* Source Control Management  
  a. Untuk bagian ini, memakai referensi [W3S](https://www.w3schools.com/git/git_staging_environment.asp?remote=github), terdapat 4 command di GIT yang akan dijelaskan, yakni:
    * git.init:  
      >Menciptakan / memulai folder .git tersembunyi didalam folder code kita, melacak sejarah codingan kita
  
      Dalam contoh, kita menggunakan **mkdir project001** di git untuk menciptakan folder kita (cara mudahnya pakai tombol new folder aja), lalu di git, pakai **cd project001** untuk masuk kedalamnya, lalu kita bisa menggunakan **git.init** untuk menciptakan .git folder didalamnya
    * git.add:  
      >Menambahkan file kedalam .git kita sehingga terlacak sejarah codingnya

      Contohny adalah dengan file ini. Saya gunakan Index.html (Some random code) dan dengan menggunakan git.add, kita dapat memasukkannya kedalam git sehingga terlacak codingnya. Gambarannya ada di lampiran
    * git.status:
      >Mengecek apakah file dalam foldernya itu untracked atau tracked.

       Tracked & untracked analoginya disave atau tidak disave. Kalau untracked artinya versi sebelumnya dari code itu akan hilang ketika diubah, sementara tracked artinya versi sebelumnya akan dijaga. Dari contoh kita diatas, mengingat file Index.html kita sudah ditambah, maka ketika kita cek, akan terlacak sebagai tracked
    * git restore --staged file / git rm --cached file
      >Untrack file yang sebelumnya ditrack pakai command git add

      Bila dalam pengerjaan kita, kita masukkan kode salah kedalam .git folder kita, maka kita keluarkan dia dari .git folder menggunakan command ini
  
  b. Connect Git and VSCode to Github  
  Pretty good here, thank you kepada link tutorial yang dikasih.[Link Tutorial](https://code.visualstudio.com/docs/sourcecontrol/github) nya disini
  
  c. Do Git Branching  
  Answers ada di lampiran, lots of weird terms, harus membiasakan diri dengan latihan proyek

  d. Learn SSH between Git and Github  
  Quite difficult, but thankfully, i did it. Answers ada di lampiran
* Pengenalan Ground Control Station  
  a. Installing Mission Planner
  Not too bad, used the [official website](https://ardupilot.org/planner/docs/mission-planner-installation.html) to download it
* Development Environment
* Dasar-Dasar UAV (Referensinya [ini](https://novapublishers.com/wp-content/uploads/2020/10/Unmanned-Aerial-Vehicles.pdf#page=9.22))
  
  a. VTOL, HTOL, and Hybrid  
  **VTOL** (Vertical Takeoff and Landing): UAV yang mirip kyk helikopter, mayoritas menggunakan alat penggerak mirip kayak helikopter (baling-baling), dan dari namanya, naik vertikal dan mendarat vertikal seperti helikopter.  
  **HTOL** (Hovering Takeoff and Landing): UAV yang mirip kyk pesawat, menggunakan alat penggerak mirip pesawat (engine pesawat, etc), dan memerlukan runway untuk dapat meluncur dan mendarat.  
  Hybrid: Kombinasi keduanya.
    
  Untuk perbedaannya, pretty clear from here. VTOL mekanisme pergerakannya mirip kyk helicopter, pergerakan alaminya naik-turun sehingga ckp enak dipakai dalam lingkungan yang sempit dibanding HTOL yang memerlukan landasan horizontal ckp dulu untuk bisa terbang, hal itu dikarenakan pergerakannya lebih mengikuti pesawat.
   
  Di sisi lain, HTOL memerlukan energi lebih sedikit dibanding VTOL dan memiliki efisiensi bahan bakar ckp tinggi sehingga waktu airbornenya lebih lama dibanding VTOL.
  
  Meskipun begitu, VTOL masih lebih populer dibanding HTOL karena dapat naik tanpa perlu bergerak dulu, making them more manouverable and easier to control

  b. Pitch, Roll, Yaw & Air Speed, Ground Speed & HDOP & RSSI  
  Pitch, Roll, Yaw singkatnya rotasi terhadap 3 sumbu arah kita. Pitch mengatur hidung UAV apa keatas/kebawah, Roll jelas seberapa miring pesawat kita, bayangin arah roll seperti arah silinder gelinding, lalu silindernya merupakan bodi UAV, dan terakhir Yaw itu seberapa kiri/kanan arah hidung UAV kita. Ilustrasinya sebagai berikut  
  ![Pitch,Roll,Yaw UAV](https://www.aviationfile.com/wp-content/uploads/2020/05/yaw-pitch-roll-1024x579.jpg)

  Air Speed & Ground Speed (Using [this](https://www.grc.nasa.gov/www/k-12/airplane/move.html) as reference)  
  Ground Speed: Speed relative to the ground, it's the one we're used to measuring as how we normally measure speed is always respect to the ground  
  Air Speed: Speed relative to the air around the UAV, it's just the ground speed of the UAV and then we either reduce or increase it by the wind speed around the UAV so that it becomes with respect to the air around instead of the ground  
![Airspeed vs Groundspeed diagram](https://tse3.mm.bing.net/th/id/OIP.tCxBdBTmEfsD3SvJnGUWQQHaFj?rs=1&pid=ImgDetMain&o=7&rm=3)  
  If the wind speed is in the same direction, then the airspeed of the UAV will be ground - wind, and vice versa, if the wind speed is in the opposite direction, then the airspeed will be ground + wind

  HDOP in GPS's (Using [this](https://www.marinepublic.com/blogs/training/649465-hdop-pdop-gdop-gps-accuracy-multipath-effects))
  DOP (Dilution of Precision) mengukur seberapa nilai error yang dimiliki satelit dalam menentukan posisi kita, semakin kecil nilainya, error lokasi kita semakin kecil sehingga pinpointnya lebih pas. Utk HDOP sendiri berfokus ke error lokasi kita terhadap lintang dan bujur kita (Posisi Horizontal, itu asal H nya), pasangannya, VDOP mengukur error posisi kita terhadap altitude (ketinggian, hence Vertical)  
  RSSI in UAV Telecommunication
  
* Algoritma
  A & D star:
  A star 
  










