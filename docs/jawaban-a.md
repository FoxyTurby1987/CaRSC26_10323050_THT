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
  <img width="1417" height="847" alt="Screenshot 2026-01-20 174616" src="https://github.com/user-attachments/assets/2e6fdbcc-d834-4772-a8c0-a4a6a7451d77" />  

  b. Features in Mission Planer  
  Some of the features are: (From [here](https://ardupilot.org/planner/docs/mission-planner-features.html))
  * CONNECT:  
    Connect Mission Planer to an autopilot (i.e. ArduPilot), is at the upper right corner of the screen
    
  * DATA:  
    Displays essential flight information (It's where the HUD, Flight Path, etc is at)
    <img width="1416" height="860" alt="Screenshot 2026-01-21 142315" src="https://github.com/user-attachments/assets/40571871-0b09-4eff-8c16-f68be463f470" />

  * PLAN:  
    Like the name, is meant to chart a course for the UAV (create the flight path)  
    <img width="1418" height="857" alt="Screenshot 2026-01-21 142325" src="https://github.com/user-attachments/assets/4b3d5530-2288-4c09-b3b9-04dc15763ac3" />

  * SETUP:  
    Where the firmware and the hardware are downloaded and installed
    <img width="1417" height="857" alt="Screenshot 2026-01-21 142336" src="https://github.com/user-attachments/assets/9d46c95d-8a42-49ba-8c79-f19bdb0e8f99" />

  c. Creating a flight path in Mission Planer
  The final results of the Flight Path (100 x 80m)
  <img width="1148" height="551" alt="Screenshot 2026-01-21 145741" src="https://github.com/user-attachments/assets/7c2040c6-299a-4f80-b212-63a62d54b753" />
  

* Development Environment  
  a. Aku coba pakai VM, namun screennya selalu hitam. Jadilah pakai WSL, sudah dapat, dan terimakasih ke [link](https://www.geeksforgeeks.org/installation-guide/how-to-install-pip-in-ubuntu/) ini, buatin downlaod semua itu mudah

<img width="1088" height="224" alt="Screenshot 2026-01-22 134926" src="https://github.com/user-attachments/assets/8878a966-15e1-4a83-94d9-954d8b29d113" />

<img width="1162" height="427" alt="Screenshot 2026-01-22 134853" src="https://github.com/user-attachments/assets/a7d70ff5-8954-4a51-8ba7-05c407ad3ee7" />

<img width="1100" height="342" alt="Screenshot 2026-01-22 134840" src="https://github.com/user-attachments/assets/025ee79b-c908-4a70-a907-818d17ebdfa7" />

<img width="1036" height="216" alt="Screenshot 2026-01-22 134830" src="https://github.com/user-attachments/assets/490de03d-622b-4fd5-a960-8b412994e360" />

<img width="1174" height="237" alt="Screenshot 2026-01-22 134818" src="https://github.com/user-attachments/assets/c2d07eea-00cf-4e77-a3a9-83ed52f944f5" />

  b. 
* Dasar-Dasar UAV
  a. VTOL, HTOL, and Hybrid (Referensinya [ini](https://novapublishers.com/wp-content/uploads/2020/10/Unmanned-Aerial-Vehicles.pdf#page=9.22))
  
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
  
  RSSI in UAV Telecommunication (Using [this](https://www.mdpi.com/1424-8220/23/11/5163))
  RSSI (Received Signal Strength Indicator) is from the name, pretty self explanatory, shows how strong the signal is received on the UAV

  c. Components of a UAV  
  Onboard a UAV, it consists of several key pieces, those being: (From [this](https://prezi.com/p/gvoftltscvqy/study-of-the-block-diagram-of-a-drone/) and [this](https://kesugroup.com/uav-structure-components-and-design/))  
  1. Frame  
     Gives the UAV its structure, it gives its shape and integrity  
  3. Propulsion  
     Gives its flight capabilities (HTOL,VTOL,Hybrid)  
  5. Control  
     Gives its maneuverability and stability  
  7. Payload  
     Depends on circumstance, allows the UAV to carry items, from photography to mail delivery

  For our case, assume the UAV is for mapping purposes, then:
  <img width="1460" height="427" alt="Screenshot 2026-01-22 154950" src="https://github.com/user-attachments/assets/dd712db3-45ae-41b3-a3e1-36c3adfc737d" />

  d. Interesting Research in regards to UAV's (This [paper](https://www.mdpi.com/2226-4310/12/1/36))  
  I found one and it is about optimizing the UAV's performance by adding onto their wingtips specific winglets. In the paper, the team increased the performance of their UAV by implementing winglets on their wingtips, decreasing lift-induced drag due to wingtip vortices (near the tips of the wings, the air there is made to a vortex due to the forward motion of the aircraft, creating drag, causing the UAV's speed to be affected). Their results show that the range, endurance, and battery use was improved significantly, showing a new field in UAV improvements
  
* Algoritma
  A & D star: (For A star [here](https://www.datacamp.com/tutorial/a-star-algorithm), For D star [here](https://www.numberanalytics.com/blog/mastering-d-star-algorithm-in-robotics))
  
  A star is a path finding algorithm, meant to find the shortest path between start and finish using a weighted graph, and is normally used when the conditions are static (the start and finish points don't move). While D star is essentially an upgrade to A star (named Dynamic A star), that is able to handle more dynamic environments (maybe the start and finish points can change over time)

  Proportional-Integral-Derivative (PID) (From [here](https://analogcircuitdesign.com/what-is-proportional-integral-derivative-pid-control/))

  PID is a control system that relies on the tuning of 3 weighted components (Kp,Ki,Kd). It calculates each of them then adds them up as the output. The goal is to maintain the process variable as close to the setpoint without there being oscillations with good response time

  Kalman Filter & Extended Kalman Filter (From [here](https://www.ece.iastate.edu/~namrata/EE527_Spring08/KalmanFilter.pdf) and [here](https://arxiv.org/pdf/2406.06427#page=7.82))

  Kalman filter is an algorithm that predicts and updates the state of a time-varying system based on predictions of the system model and noise observations. It uses linear relations to do so, but in most real world cases, relations are not so linear. Hence the need of an Extended Kalman Filter

  The Extended Kalman Filter (EKF) is an extension of the Kalman Filter where it takes into account non-linear relations and by using taylor expansion, approximates it into a linear model, where the usual Kalman Filter can take over

  
  
  












