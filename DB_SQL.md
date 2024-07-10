# DB SQL 　データベース基礎　研修

[データベース研修資料.pdf](./【共通】データベース基礎.pdf)

### データ型

データ型 意味
integer 整数（4 バイト）
int8 整数（8 バイト）
serial 整数(自動発番) ※主に主キーで使います
double, float 浮動小数点型
numeric 数値型（数値全体の桁数と小数部の桁数を指定）
text 文字(文字数制限無し)
varchar(n) 文字(n 文字まで)
timestamp 日付・時刻型
date 日付型
boolean 真偽値型

**自動発番** serial データが入力されると自動で番号が振られる。

**制約**　`foreign key`は現場では定義されていないケースが多い。テストするときに面倒くさいらしい

**DROP TABLE**　これは現場では絶対にやってはいけない。

## SQL コマンド

#### INSERT INTO


   複数レコードを挿入。

> `INSERT into employees 
(id,name,age,gender,department_id) 
VALUES(6,'佐藤万治',19,'男性',1),(7,'野口次郎',25,'男性',1),(8,'工藤次郎',88,'女性',1),
(9,'引地次郎',78,'女性',3),(10,'山口裕',32,'男性',2);`
