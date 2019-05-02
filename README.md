# word2vec-model-wiki
使用維基百科提供的中文資料, 先進行繁簡轉換, 再使用jieba分詞, 最後生成詞向量模型<br>
## 中文維基百科語料
https://dumps.wikimedia.org/zhwiki/latest/
## 繁簡轉換
使用OpenCC進行轉換<br>
安裝:<br>
<code>pip install opencc-python-reimplemented</code>
## 製作模型
使用gensim裡的word2vec套件<br>
<code>pip install gensim</code>
## 測試
用most_similar()找到關聯詞
<code>
  model.wv.most_similar('橄欖油', topn=20)
</code>
