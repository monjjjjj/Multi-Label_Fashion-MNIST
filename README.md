# Multi-Label_Fashion-MNIST
## 產生訓練資料集
## 使用fashion MNIST的資料集去產生multi-label的資料集
FashionMNIST資料集內總共包含10種類別的圖片(T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)     

隨機從10種類別中挑4種類別來組成一張training data，共生成10000張圖片。  
### 所生成的training data & testing data如下所示:
![1830](https://user-images.githubusercontent.com/62006029/197686250-70fc1d32-85d8-457a-8e3f-ae2a4dbc9792.png)

### 圖片生成完後的CSV檔(分別會有training_labels.csv及testing_labels.csv)內容:
![image](https://user-images.githubusercontent.com/62006029/197686747-07085abc-4fa3-4ebb-9495-3f0d529d7ac8.png)  

label: 按照10種類別順序標示圖片中實際有哪些類別
real_int: 





reference: https://github.com/f-rumblefish/Multi-Label-Fashion-MNIST
