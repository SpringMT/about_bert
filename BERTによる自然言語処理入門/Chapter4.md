Segemakerでやってみる

##注意点
### PyTorchを使う

<img width="530" alt="image" src="https://user-images.githubusercontent.com/579005/154593657-fd6582c0-f26b-408d-b3bd-8316eefe2aec.png">

### GPUを使ってない場合は

```
bert = bert.cuda() 
```
や

```
# データをGPUに載せる
encoding = { k: v.cuda() for k, v in encoding.items() } 
```
などは不要(なはず)

### インスタンス
2 vCPU 4GBのメモリだとjson loadで止まる

