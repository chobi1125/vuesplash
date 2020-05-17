## 使い方
git clone https://github.com/chobi1125/vuesplash.git

cd vuesplash

docker-compose up -d // Docker起動

docker-compose exec vuesplash_web bash // 仮想環境へ

composer install // venderが生成

cp .env.example .env // envの作成

php artisan key:generate // キーの生成

## 参考になりそう

Laravel5のプロジェクトをGitで管理する

https://qiita.com/zaburo/items/bc448a9fbf2d35194302

備忘録記事

https://chobimusic.com/docker-laravel/


## .gitignoreへの配慮

デフォルト

/node_modules // 関係なし

/public/hot // 関係なし

/public/storage // 関係なし

/storage/*.key // 関係なし

/vendor // composer iで対処

.env // コピペ？？

.env.backup // 関係なし

.phpunit.result.cache // 関係なし

Homestead.json // 関係なし

Homestead.yaml // 関係なし

npm-debug.log // 関係なし

yarn-error.log // 関係なし