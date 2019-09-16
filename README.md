#測試submodule

主要參考 這兩篇
https://blog.chh.tw/posts/git-submodule/

http://josephj.com/entry.php?id=342&fbclid=IwAR0UXyy58Z47P5TAncXOt5Dqq1AfkNfnfAwSnecTZ-5-0pMMV7Fo-NRjN4Y

#新增submodule
git submodule add xxx.git where_you_want_to_put

#抓
git clone --recursive 是clone並且把submodule也clone

若一般的clone是不會抓submodule 
需要透過
git submodule init
git submodule update --recursive

補齊submodule

#更新Submodule
git submodule foreach --recursive git pull origin master

cd到submodule folder後的git操作就是那個submodule

當更新完submodule的時候 記得要去自己的project把它git add近來