# Multi-Label_Fashion-MNIST
## 產生訓練資料集
## 使用fashion MNIST的資料集去產生multi-label的資料集
FashionMNIST資料集內總共包含10種類別的圖片(T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)     

隨機從10種類別中挑4種類別來組成一張training data和testing data，共生成10000張圖片。  
### 所生成的training data & testing data如下所示:
![1830](https://user-images.githubusercontent.com/62006029/197686250-70fc1d32-85d8-457a-8e3f-ae2a4dbc9792.png)

### 圖片生成完後的CSV檔(分別會有training_labels.csv及testing_labels.csv)內容:
![image](https://user-images.githubusercontent.com/62006029/197686747-07085abc-4fa3-4ebb-9495-3f0d529d7ac8.png)  

label: 按照10種類別順序標示圖片中實際有哪些類別

real_int: 圖片中依序出現的類別有哪些 

### 訓練過程
![1](https://user-images.githubusercontent.com/62006029/197928915-1e2063c0-e0ca-4167-8f78-dba34f69a01b.png)

圖片上方為accuracy history，下方為loss history

可觀察出初步訓練過程中準確度只能維持在30%以下，但loss都是很低的!

目前仍在思考為何準確度會只有30%? 如何提高它?

### Hint for multi-label classification 
1. 不能直接使用one-hot encoding

2. 因為是要做multi-label classification，每個類別的輸出是獨立的，因此使用binary_crossentropy

3. 模型的最後一層要使用sigmoid function而不是softmax function






reference: https://github.com/f-rumblefish/Multi-Label-Fashion-MNIST
