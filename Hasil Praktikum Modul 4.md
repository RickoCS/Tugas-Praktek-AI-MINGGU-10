Nama  : Ricko Chandra Saputra <br />
NIM   : 5311421075 <br />

**1. Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7.**<br />

Pertama Algoritma BFS ini melakukan search atau mengunjungi node 3 untuk pertama kali dengan distance yang tertulis adalah 0. Kemudian setelah mengunjungi node 3, maka selanjutnya algoritma mengunjungi node 4 dan node 2 dengan distance 1 dari jarak awal. Selanjutnya  setelah mengunjungi node 4 dan node 2, maka selanjutnya algoritma mengunjungi node 5, node 6 dan node 7 dengan distance 2 dari jarak awal. Dan yang terakhir setelah mengunjungi node 5, node 6 dan node 7 maka algoritma akan mengunjungi node ke 8 dengan distance 3. 
Dengan demikian, algoritma ini dapat menentukan node-node tersebut dengan melihat informasi tentang distance atau jarak yang disimpan untuk setiap node. Maka untuk menentukan jarak dari node awal ke node 8, node 6, dan node 7 adalah dengan cara melihat nilai distance dari node 8, yaitu 2 dan 3. <br />

Dengan demikian, algoritma ini dapat menentukan node-node tersebut dengan melihat informasi tentang distance atau jarak yang disimpan untuk setiap node. Maka untuk menentukan jarak dari node awal ke node 8, node 6, dan node 7 adalah dengan cara melihat nilai distance dari node 8, yaitu 2 dan 3. Untuk lebih jelasnya dapat dilihat pada hasil program berikut.<br />

"(3,d=0) (4,d=1) (2,d=1) (5,d=2) (6,d=2) (1,d=2) (7,d=3) (8,d=3)"<br />
**2. Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.5 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5.**<br />

Untuk menentukan node 5 dengan menggunakan algoritma BFS maka algoritma akan melakukan pencarian (search) atau menjelajah pertama kali pada node 0, Kemudian dilanjutkan dengan melakukan pencarian pada node selanjutnya hingga ke node terakhir. Maka setelah dilakukan pencarian maka didapatkan node 5 dengan jarak BFS sebesar 2 dari node awal. Untuk lebih jelasnya dapat dilihat pada hasil program berikut.<br /> 

"(0,d=0) (1,d=1) (2,d=1) (3,d=2) (4,d=2) (5,d=2) (6,d=2)"<br />
**3. Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.6 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 9.**<br />

Untuk menentukan node 9 dengan menggunakan algoritma BFS maka algoritma akan melakukan pencarian (search) atau menjelajah pertama kali pada node 1, Kemudian dilanjutkan dengan melakukan pencarian pada node selanjutnya hingga ke node terakhir. Maka setelah dilakukan pencarian maka didapatkan node 9 dengan jarak BFS sebesar 3 dari node awal. Untuk lebih jelasnya dapat dilihat pada hasil program berikut.<br /> 

"(1,d=0) (2,d=1) (3,d=1) (4,d=1) (5,d=2) (6,d=2) (7,d=2) (8,d=2) (9,d=3) (10,d=3) (11,d=3) (12,d=3)"<br />
**4. Ubahlah kode program di atas sehingga bentuk tree seperti Gambar 4.7 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node C**<br />
Pada percobaan ini akan dilakukan permisalah bahwa node A= 1, node B =2, node C = 3 dan seterusnya sampai node 9 = I. Maka untuk menentukan node 3 dengan menggunakan algoritma BFS maka algoritma akan melakukan pencarian (search) atau menjelajah pertama kali pada node F (6), Kemudian dilanjutkan dengan melakukan pencarian pada node selanjutnya hingga ke node terakhir. Maka setelah dilakukan pencarian maka didapatkan node C (3) dengan jarak BFS sebesar 3 dari node awal. Untuk lebih jelasnya dapat dilihat pada hasil program berikut.<br /> 

"(6,d=0) (2,d=1) (7,d=1) (1,d=2) (4,d=2) (9,d=2) (3,d=3) (5,d=3) (8,d=3)"<br />
