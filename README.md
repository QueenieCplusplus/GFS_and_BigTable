# GFS and BigTable （ HBase ）

Google advocated GFS in 2003 and then introduce HBase in 2007.
Facebook in 2010, and Apach rleased Open Source in 2013. 

# 學術發表

2003 年，由 Google 發表 GFS 論文。

# 核心存儲技術

core tech : 將資料儲存於不同的資料節點上！資料是以時間戳記搭配 K/V，集合是以 Key 所排序的，而每一個值都有不同的 Timestamps 與其對應。


        GFS -> BigTable -> HDFS -> HBase
        
# HDFS

全名為 Hadoop File System，作為 Hadoop 基底設施，將 HDFS 上所有檔案切成 Chunk (以前稱為 Block) 的資料區塊，並搭配容錯效用的 Replication Factor 複製因數。此因數越大，容錯率越高，然而也越浪費資源。


# 臉書案例

2010 年，臉書實現了 2300 個 Hadoop 叢集，儲存 40 PB 資料量！

# 開源版本

2013 年，Apache Hadoop 1.0 版本釋出～

其他版本尚有 Cloudera & Hortonworks。




