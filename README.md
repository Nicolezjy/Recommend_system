# hw5_推荐系统


### 数据：Million Song Dataset(MSD)


 https://labrosa.ee.columbia.edu/millionsong/
 公开音乐数据集 Million Song Dataset(MSD) ， 它 包 含 来 自 SecondHandSongs dataset 、 musiXmatch dataset、Last.fm dataset、Taste Profile subset、 thisismyjam-to-MSD mapping、tagtraum genre annotations 和 Top MAGD dataset 七个知名音乐社区的数据。
原始数据集包括：
1.	train_triplets.txt：三元组数据（用户、歌曲、播放次数）
2.	track_metadata.db：每个歌曲的元数据
由于原始数据太大，作业用的数据集只是其中的子集（播放次数最多的10万个用户、播放次数最多的3万首歌曲。
数据预处理过程请见DataProcessing.ipynb文件，最后得到的数据文件为：triplet_dataset_sub_song_merged.csv（1千万条记录）

### 功能要求


将triplet_dataset_sub_song_merged.csv中的数据用train_test_split分成60%数据做训练，剩下40%数据做测试。
1.	实现基于用户的协同过滤； 
2.	实现基于物品的协同过滤；
3.	实现基于模型（矩阵分解/LFM）的协同过滤。
4.	对每种推荐算法的推荐结果，用Top20个推荐歌曲的准确率和召回率评价推荐系统的性能。


