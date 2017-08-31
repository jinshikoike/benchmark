# CPUベンチマーク

# 指標
大きく分けて二つ  
## スピード
ある単位のタスクをどれくらい早く完了できるか。  

## スループット
単位時間あたりにどれだけのタスクを完了できるか。  

---

# 種類
どんなものがあるか調査してみた。他にもいっぱいあるっぽい。  

## CPI(Clock|cycles per instruction)
一つの命令を実行するのにCPUクロック周期が何サイクル必要かを表したもの。  
この値が小さければ小さいほど良い  

## MIPS(Million Instructions per second)
毎秒何百万個の命令が実行できるかを表す。  
MIPSは、同じ命令セットを持つCPU同士で性能を比べないと意味がない。同じことをするのに必要な命令の数が異なるからである  

## FLOPS(Floating Point Operation per Second)
一秒間に浮動小数点演算が何回できるかの指標  
化学計算など、高度な精度が必要な計算の際にこの指標が重要になってくる。  

## SPEC(Standard Performance Evaluation Corporation:標準性能評価法人)
コンピュータの公平で意味のあるベンチマークを作成する事を目指して設立された非営利団体  
SPECのベンチマークは「現実の」状況をテストする事を目指す。  
SPECが公開してるベンチマークにはいろいろな種類がある。  
例えばWebサーバの性能評価のためにHTTPリクエストを並列して行う、SpecwebやCPU性能を評価するためのSpecCPUなど。  

ここが参考になる。  
- [SPECの見方](http://qiita.com/s2maeda/items/b07364fd94fbd3ac0ef4)

### SPEC Speed metric
一つのタスクを完了するのにかかった時間を評価した時間.  

### SPEC rate metric
複数のタスクを同時に実行した時のスループットの合計から評価した結果.  

---

# [UnixBench](https://github.com/kdlucas/byte-unixbench)
http://blog.idcf.jp/entry/cloud/unixbench/
http://naoberry.com/tech/unixbench/

# SysBench
http://knowledge.sakura.ad.jp/tech/1048/3/


# Refference
http://knowledge.sakura.ad.jp/tech/1048/
