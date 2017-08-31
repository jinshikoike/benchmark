# Storage BenchMark

# Index

## read/write speed.

But read/write performance differ depending on access method.  
Generally, It is said that sequential access is most high performance.  
Sequential access is to write sequential data at once.  
On the other hand, random access is less performance than sequential access.  
Rodom access it to write little into data random location.  

# Tool

- hdparm
- Bonnie++
- dbench
- fs_mark
- tiobench
- IOzone
- fio

## note
キャッシュの影響を小さくするためには、テストに使用するファイルの総サイズを搭載する物理メモリの総量よりも大きく。  
ベンチマークツールによって異なるが、搭載物理メモリの2倍程度が目安らしい。  
また、Linuxの場合、起動時のカーネルパラメータで「mem=＜メモリ容量＞」というオプションを指定することで、使用するメモリ量を制限できる。  
これを利用して、ベンチマークテスト時にはあえて利用できるメモリ容量を少なくする場合もある。たとえば搭載しているメモリのうち256MBのみを使用するには、起動時に以下のようなカーネルオプションを指定すれば良い。  

`mem=256M`

詳しくはRefferenceのリンクを参照。

# hdparm
https://www.server-world.info/en/note?os=CentOS_7&p=hdparm  

- `yum -y install hdparm`
- `hdparm -t /dev/sda`
-tオプションはキャッシュなし読み込み速度


#Bonnie++


# Refference
http://knowledge.sakura.ad.jp/tech/938/2/

