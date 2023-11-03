Nama : Ricko Chandra Saputra <br />
NIM  : 5311421075 <br />

**TEKNIK HEURISTIC SEARCH**<br />

**1.	Pelajari class EightPuzzleSearch, EightPuzzleSpace, dan Node.**<br />
Class EightPuzzleSearch merupakan salah satu class yang bertanggung jawab untuk melakukan pencarian heuristic dengan menggunakan fungsi biaya (cost function) atau bekerja sesuai dengan algoritma heuristic. Pada class ini algoritma heuristic dapat  menyimpan node-node yang belum dan sudah dikunjungi. Selain itu, pada class ini algoritma heuristic dapat mencetak alur (path) dari root ke suatu node, dan menentukan node terbaik berdasarkan nilai dari fungsi heuristic.<br />

Class EightPuzzleSpace: merupakan salah satu class yang dapat menggambarkan ruang keadaan dari game 8-puzzle. Gambaran tersebut dapat berupa susunan ubin-ubin angka dari 0 sampai 8. Kemudian class ini juga memiliki method untuk mengembalikan node akar (root) dan node tujuan (goal), serta method untuk menghasilkan node-node penerus (successor) dari suatu node dengan melakukan operasi geser ubin ke atas, bawah, kiri, atau kanan.<br />

Class Node: Class ini merepresentasikan sebuah node dalam ruang pencarian, yang memiliki atribut state, cost, parent, dan successors. State adalah sebuah array dari integer yang menyimpan susunan ubin-ubin angka pada node tersebut. Cost adalah nilai biaya yang dihitung dengan menggunakan fungsi heuristic. Parent adalah node induk dari node tersebut, sedangkan successors adalah vektor dari node-node penerus yang dihasilkan dari operasi geser ubin.<br />

Kemudian berikut merupakan hasil dari percobaan point 1.<br />

“Root: 3 1 2 4 7 5 6 8 0<br /> 
Solution found<br />
 3 1 2 4 7 5 6 8 0<br /> 
 3 1 2 4 7 5 6 0 8 <br />
 3 1 2 4 0 5 6 7 8 <br />
 3 1 2 0 4 5 6 7 8 <br />
 0 1 2 3 4 5 6 7 8<br />
BUILD SUCCESSFUL (total time: 0 second)”<br />

Berdasarkan hasil diatas maka dapat dilihat bahwa initial state pada 8-puzzle diatas adalah [ 3 1 2 4 7 5 6 8 0 ] dan goal statenya adalah [0 1 2 3 4 5 6 7 8]. Dari hasil diatas, algoritma heuristic dapat memecahkan kasus pada 8-puzzle dengan mengubah keadaan awal (initial) menjadi sesuai dengan tujuan yang telah ditentukan(goal state). 
Untuk menemukan solusi atau memecahkan kasus 8-puzzle menjadi sesuai dengan tujuan yang telah ditentukan dibutuhkan proses hingga 5 langkah. Dan juga algoritma heuristic tersebut hanya membutuhkan waktu 0 second untuk mencapai tujuan (goal state).<br />  

**2.	Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 8. 
Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1.**<br />

Pada percobaan ini didapatkan hasil sebagai berikut.<br />

“Root: 3 1 2 4 7 5 6 8 0 <br />
Solution found<br />
 3 1 2 4 7 5 6 8 0 <br />
 3 1 2 4 7 5 6 0 8 <br />
 3 1 2 4 0 5 6 7 8 <br />
 3 1 2 0 4 5 6 7 8 <br />
 0 1 2 3 4 5 6 7 8 <br />
 1 0 2 3 4 5 6 7 8 <br />
 1 2 0 3 4 5 6 7 8 <br />
 1 2 5 3 4 0 6 7 8 <br />
 1 2 5 3 0 4 6 7 8 <br />
 1 2 5 0 3 4 6 7 8 <br />
 0 2 5 1 3 4 6 7 8 <br />
 2 0 5 1 3 4 6 7 8 <br />
 2 3 5 1 0 4 6 7 8 <br />
 2 3 5 1 4 0 6 7 8 <br />
 2 3 0 1 4 5 6 7 8 <br />
 2 0 3 1 4 5 6 7 8 <br />
 0 2 3 1 4 5 6 7 8 <br />
 1 2 3 0 4 5 6 7 8 <br />
 1 2 3 4 0 5 6 7 8 <br />
BUILD SUCCESSFUL (total time: 1 second)”<br />

Berdasarkan hasil diatas maka dapat dilihat bahwa initial state pada 8-puzzle diatas adalah [ 3 1 2 4 7 5 6 8 0 ] dan goal statenya adalah [1 2 3 4 0 5 6 7 8]. 
Dari hasil diatas, algoritma heuristic dapat memecahkan kasus pada 8-puzzle dengan mengubah keadaan awal (initial) menjadi sesuai dengan 
tujuan yang telah ditentukan (goal state). Untuk menemukan solusi atau memecahkan kasus 8-puzzle menjadi sesuai dengan tujuan (goal state) 
yang telah ditentukan dibutuhkan proses hingga  19 langkah.<br />

Perbedaan dengan percobaan pada point satu adalah pada percobaan ini algoritma heuristic membutuhkan proses yang cukup panjang untuk 
mencapai tujuan (goal state). Proses tersebut membutuhkan hingga 19 langkah, yang dimana proses tersebut cukup panjang daripada 
percobaan point 1 yang hanya 5 langkah. Maka dari itu algoritma heuristic pada percobaan ini membutuhkan waktu lama hingga 1 second yang
dimana waktu tersebut lebih lama dibandingkan dengan point 1 yang hanya 0 second. Dan juga algoritma heuristic ini 
akan membutuhkan memori yang besar untuk mencapai tujuan (goal state) karena membutuhkan waktu yang lama dan langkah yang begitu banyak.<br />   

**3.	Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.9. 
Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1 dan 2.**<br />

Pada percobaan ini didapatkan hasil sebagai berikut.<br /> 

“Root: 1 5 3 4 6 8 2 7 0 <br />
BUILD STOPPED (total time: 55 minutes 45 seconds)”<br />

Berdasarkan hasil diatas dapat dilihat bahwa initial pada 8-puzzle diatas adalah [1 5 3 4 6 8 2 7 0] dan goal statenya adalah [7 6 5 8 0 4 1 2 3]. 
Pada percobaan diatas algoritma heuristic tidak dapat menemukan solusi untuk mengubah initial menjadi goal state. 
Hal tersbeut dapat dilihat bahwa hingga waktu mencapai 55 menit, algoritma heuristic belum juga menemukan solusi. 
Sehingga perbedaan dari point 1 dan 2 adalah pada point 3 ini algoritma heuristic tidak dapat menemukan solusi terbaik untuk mencapai tujuan (goal state)<br />  

**4.	Ubahlah Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.10. 
Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1, 2, dan 3.**<br />

Pada percobaan ini didapatkan hasil sebagai berikut.<br />

“Root: 1 2 3 4 5 6 7 8 0<br /> 
Solution found<br />
 1 2 3 4 5 6 7 8 0 <br />
 1 2 3 4 5 6 7 0 8 <br />
 1 2 3 4 0 6 7 5 8 <br />
 1 2 3 4 6 0 7 5 8 <br />
 1 2 0 4 6 3 7 5 8 <br />
 1 0 2 4 6 3 7 5 8 <br />
 0 1 2 4 6 3 7 5 8 <br />
 4 1 2 0 6 3 7 5 8 <br />
 4 1 2 6 0 3 7 5 8 <br />
 4 1 2 6 5 3 7 0 8 <br />
 4 1 2 6 5 3 0 7 8 <br />
 4 1 2 0 5 3 6 7 8 <br />
 0 1 2 4 5 3 6 7 8 <br />
 1 0 2 4 5 3 6 7 8 <br />
 1 2 0 4 5 3 6 7 8 <br />
 1 2 3 4 5 0 6 7 8 <br />
 1 2 3 4 0 5 6 7 8 <br />
BUILD SUCCESSFUL (total time: 0 seconds)”<br />

Berdasarkan hasil diatas maka dapat dilihat bahwa initial state pada 8-puzzle diatas adalah [ 1 2 3 4 5 6 7 8 0 ] dan goal statenya adalah [1 2 3 4 0 5 6 7 8]. Dari hasil diatas, algoritma heuristic dapat memecahkan kasus pada 8-puzzle dengan mengubah keadaan 
awal (initial) menjadi sesuai dengan tujuan yang telah ditentukan (goal state). Untuk menemukan solusi atau memecahkan kasus 8-puzzle menjadi sesuai dengan tujuan (goal state) yang telah ditentukan dibutuhkan proses hingga  17 langkah. 
Dan juga algoritma heuristic tersebut hanya membutuhkan waktu 0 second untuk mencapai tujuan (goal state).<br />

Perbedaan pada percobaan ini dengan point 1, 2, dan 3 adalah pada banyaknya langkah yang dibutuhkan untuk mencapai tujuan (goal state). Langkah yang dibutuhkan pada percobaan ini lebih banyak dibandingkan 
dengan point 1 dan lebih sedikit dibandingkan dengan 2. Namun pada percobaan ini lebih baik dibandingkan dengan point 3 yang tidak dapat ditemukan solusi untuk mencapai tujuan *goal state”.<br /> 

**5.	Ubahlah initial dan goal state dari program dan class-class di atas sehingga bentuk initial dan goal statenya Gambar 5.11. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state.**<br />

Pada percobaan ini akan menggunakan angka untuk mewaklikan hurf A, B, C, hingga H. Misalnya A = 1, B = 2, C = 3, hingga H = 8. Kemudian hasil dari percobaan ini adalah sebagai berikut.<br />

“Root: 4 2 5 1 6 7 8 3 0<br /> 
BUILD STOPPED (total time: 54 minutes 13 seconds)”<br />

Berdasarkan hasil diatas dapat dilihat bahwa initial state pada 8-puzzle diatas adalah [ 4 2 5 1 6 7 8 3 0 ] dan goal statenya adalah [1 8 7 2 0 6 3 4 5]. Kemudian untuk hasil dari percobaan diatas adalah algoritma heuristic 
tidak dapat menemukan solusi untuk mencapai tujuan (goal state) yang telah ditentukan hingga memakan waktu 54 menit. 
Beberapa hal yang menyebabkan algoritma heuristic tidak dapat menemukan solusi adalah algoritma heuristic memiliki keterbatasan dalam menangani ketidakpastian atau ambiguitas dalam pernyataan masalah atau data yang tersedia. 
Dan juga kelemahan dari algoritma heuristic adalah dimana pencarian solusi menggunakan algoritma heuristic akan ditemukan dengan baik namun bisa juga kemungkinan tidak ada solusi.<br /> 

