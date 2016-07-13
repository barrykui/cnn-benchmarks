# cnn-benchmarks

All benchmarks were run on the same machine. The benchmark machine has dual Intel Xeon E5-2630 v3 processors
(8 cores each plus hyperthreading means 32 threads) and 64GB RAM and is running Ubuntu 14.04 with the CUDA 8.0 Release Candidate.

### alexnet (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|7.36|7.36|23.18|
|GeForce GTX TITAN X (cuDNN 5005)|7.02|7.02|23.71|
|Tesla K40c (cuDNN 5005)|18.32|18.32|61.48|


### vgg16 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|66.56|66.56|232.55|
|GeForce GTX TITAN X (cuDNN 5005)|76.15|76.15|262.42|
|GeForce GTX 1080 (nn)|143.81|143.81|522.42|
|GeForce GTX TITAN X (nn)|172.56|172.56|587.97|
|Tesla K40c (cuDNN 5005)|265.77|265.77|920.21|
|Tesla K40c (nn)|340.79|340.79|1231.01|
|CPU: Dual Intel Xeon E5-2630 v3|3101.76|3101.76|8495.48|


### vgg19 (input 16 x 3 x 224 x 224)  

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|80.39|80.39|281.69|
|GeForce GTX TITAN X (cuDNN 5005)|93.83|93.83|323.40|
|GeForce GTX 1080 (nn)|176.45|176.45|630.08|
|GeForce GTX TITAN X (nn)|215.55|215.55|709.88|
|Tesla K40c (cuDNN 5005)|325.18|325.18|1129.65|
|Tesla K40c (nn)|416.65|416.65|1475.02|
|CPU: Dual Intel Xeon E5-2630 v3|3609.78|3609.78|9849.23|


### resnet-18 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|14.69|14.69|47.07|
|GeForce GTX TITAN X (cuDNN 5005)|16.97|16.97|53.84|
|GeForce GTX 1080 (nn)|43.05|43.05|122.00|
|GeForce GTX TITAN X (nn)|55.20|55.20|150.76|
|Tesla K40c (cuDNN 5005)|51.07|51.07|168.30|
|Tesla K40c (nn)|97.85|97.85|308.91|
|CPU: Dual Intel Xeon E5-2630 v3|847.46|847.46|2195.78|


### resnet-34 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|24.83|24.83|79.70|
|GeForce GTX TITAN X (cuDNN 5005)|28.72|28.72|91.94|
|GeForce GTX 1080 (nn)|84.27|84.27|222.31|
|GeForce GTX TITAN X (nn)|109.75|109.75|274.69|
|Tesla K40c (cuDNN 5005)|95.11|95.11|303.80|
|Tesla K40c (nn)|190.80|190.80|571.37|
|CPU: Dual Intel Xeon E5-2630 v3|1530.01|1530.01|3965.21|


### resnet-50 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|50.67|50.67|153.90|
|GeForce GTX TITAN X (cuDNN 5005)|56.42|56.42|171.02|
|GeForce GTX 1080 (nn)|109.81|109.81|311.47|
|GeForce GTX TITAN X (nn)|136.37|136.37|382.36|
|Tesla K40c (cuDNN 5005)|129.21|129.21|449.90|
|Tesla K40c (nn)|250.91|250.91|769.79|
|CPU: Dual Intel Xeon E5-2630 v3|2477.61|2477.61|6627.25|


### resnet-101 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|77.77|77.77|235.33|
|GeForce GTX TITAN X (cuDNN 5005)|88.30|88.30|260.12|
|GeForce GTX 1080 (nn)|203.33|203.33|524.93|
|GeForce GTX TITAN X (nn)|258.26|258.26|662.42|
|Tesla K40c (cuDNN 5005)|220.92|220.92|797.89|
|Tesla K40c (nn)|477.37|477.37|1373.07|
|CPU: Dual Intel Xeon E5-2630 v3|4414.91|4414.91|11306.24|


### resnet-152 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX 1080 (cuDNN 5005)|109.93|109.93|328.90|
|GeForce GTX TITAN X (cuDNN 5005)|125.69|125.69|366.97|
|GeForce GTX 1080 (nn)|299.12|299.12|760.07|
|GeForce GTX TITAN X (nn)|379.79|379.79|959.42|
|Tesla K40c (cuDNN 5005)|319.80|319.80|1146.73|
|Tesla K40c (nn)|700.24|700.24|1982.23|
|CPU: Dual Intel Xeon E5-2630 v3|6572.17|6572.17|16872.78|


### resnet-200 (input 16 x 3 x 224 x 224)

|GPU|Forward (ms)|Backward (ms)|Total (ms)|
|---|---|---|---|
|GeForce GTX TITAN X (cuDNN 5005)|171.15|171.15|493.82|
|GeForce GTX TITAN X (nn)|491.69|491.69|1298.65|
|Tesla K40c (cuDNN 5005)|428.03|428.03|1485.24|
|Tesla K40c (nn)|891.46|891.46|2578.20|
|CPU: Dual Intel Xeon E5-2630 v3|8666.43|8666.43|22425.16|