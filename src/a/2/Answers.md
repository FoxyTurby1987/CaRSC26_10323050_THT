A: Commands in Git  
git init
1. Ciptakan folder lalu masuk ke foldernya (mkdir -> cd)  
<img width="511" height="118" alt="Screenshot 2026-01-20 151703" src="https://github.com/user-attachments/assets/62bb6383-03c1-4d62-9a07-29ae373c0083" />

2. Lalu pakailah git init untuk menciptakan .git folder (invisible)  
<img width="871" height="75" alt="Screenshot 2026-01-20 151720" src="https://github.com/user-attachments/assets/db056593-4f35-4623-94aa-6df39382a8fc" />

git add    
1. Didalam foldernya, perlu ada file untuk diadd ke git, maka dari itu, buatlah file simple untuk dimasukin folder  
<img width="478" height="232" alt="Screenshot 2026-01-21 134038" src="https://github.com/user-attachments/assets/9fc1cb80-cbc5-44d3-b474-ace9d34bd35b" />

2. Kalau sudah masuk foldernya, langsung saja input command git add utk memasukinya ke git folder
<img width="621" height="61" alt="Screenshot 2026-01-21 133437" src="https://github.com/user-attachments/assets/a763cae2-581e-43ff-8fc4-f5c210780a39" />  

git status
1. Langsung aja, ketikkan command git status ke terminal untuk mengecek apakah ada file yang kelacak git. Dalam kasus kita akan ada 2 kasus, ketika sebelum diadd Index.html dan yang sesudah. Yang sebelum akan menunjukkan Index.html untracked, sementara yang sesudah akan menunjukkan Index.html tracked  
<img width="746" height="198" alt="Screenshot 2026-01-21 133501" src="https://github.com/user-attachments/assets/ea0ab62e-aa9e-45b7-8de7-719dec5fa369" />
<img width="590" height="209" alt="Screenshot 2026-01-21 133449" src="https://github.com/user-attachments/assets/37f25e97-db6e-4ee0-b54c-a1fb045fca6c" />  

git restore --staged file
1. Bila ada file yang ingin diuntracked lagi, pakailah pada filenya. In this case, kita gunakannya untuk untrack Index.html    
2. Terkadang command ini tidak bekerja sehingga perlu memakai command lain untuk untrack filenya (biasanya disuggest di bagian git status, lihat lagi di fotonya diatas) yaitu git rm --cached file  
<img width="599" height="77" alt="Screenshot 2026-01-21 134837" src="https://github.com/user-attachments/assets/9c0e20b7-eb17-4292-b2f2-7e03af306eec" />

B: Set up Github dengan VSCode  
<img width="387" height="1042" alt="Screenshot 2026-01-20 154604" src="https://github.com/user-attachments/assets/b110b197-ab2f-42ab-9d8b-4b12a712aab0" />

C: Finish Git Branching (Main 4, Remote 6)  
<img width="930" height="236" alt="Screenshot 2026-01-20 164858" src="https://github.com/user-attachments/assets/d8bb9861-af8f-43b3-ac19-fd9c1dc52674" />  
<img width="1035" height="357" alt="Screenshot 2026-01-20 170705" src="https://github.com/user-attachments/assets/9825705a-3639-47eb-ba2e-2b5d9f0b70ee" />

D: SSH between Git and Github  
<img width="1217" height="870" alt="Screenshot 2026-01-20 173002" src="https://github.com/user-attachments/assets/2733c7c8-b97b-4c47-9499-d3912cba8455" />
