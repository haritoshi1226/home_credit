# 目的
データサイエンス勉強会 at 電通にて、[kaggle Home Credit Default Risk](https://www.kaggle.com/c/home-credit-default-risk)用のGit  

# フォルダ構成
|- data  
　　|- application_test.csv  
　　|- application_train.csv  
　　|- bureau.csv  
　　|- bureau_balance.csv  
　　|- credit_card_balance.csv  
　　|- HomeCredit_columns_description.csv  
　　|- installments_payments.csv  
　　|- POS_CASH_balance.csv  
　　|- previous_application.csv  
　　|- sample_submission.csv  
|- home_credit(Git)  
　　|- README.md(this)  
　　|- 各自の名前ディレクトリ

# 使用方法
1. このレポジトリをクローンする 

~~~
    git clone git@github.com:haritoshi1226/home_credit.git
~~~
2. 梁木に自分のGitHubアカウントをSlackで知らせる
3. 自分のディレクトリが作成されたら、その中に分析コードを書く  

# 運用
変更をGitHubにpushする際は、自分のブランチを作成し、そこにコミットする  
その後masterに自分のブランチをマージし、GitHubにpushする  
1. ブランチの作成  
hogehogebranchの部分に自分の名前のbranch名を入れてブランチを作成する   
~~~
    git branch hogehogebrunch 
~~~ 
2. ブランチの切り替え  
ブランチを先ほど作成したブランチに切り替える
~~~
    git checkout hogehogebranch
~~~
3. 自分のブランチにコミット  
自分のブランチ内に、更新結果をコミットする
~~~
    git add -A
    git commit -m 'hogehoge'
~~~
4. マージ  
ブランチを「master」に切り替え、マージし、GitHubにpushする  
git pullコマンドを実行した際、自分の変更した分は一旦消えてしまうため、必ず自分のブランチであらかじめcommitをしておくこと
~~~
    git checkout master
    git pull master
    git merge hogehogebrunch
    git push origin master
~~~

5. 2〜4を繰り替えす