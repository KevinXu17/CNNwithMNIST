# CNNwithMNIST

### Why CNN not FF
FF can not handle large num of features like picture pixels.

### Layer
1. CNN: input, kernel size 8, stride 1, padding 1 => 
((input + 2 * padding - kernel)/stride + 1) output 8 channels 28*28 map; BatchNorm; ReLU 
2. MaxPool:  size 2 => 28 /2 = 14*14 map
3. CNN: kernel size 5, stride 1, padding 2 => output 32 channels 14 * 14 map; BatchNorm; ReLu
4. MaxPool: size 2 => 7*7 map
5. Linear: 7*7*32 => 600
6. drop out
7. Linear