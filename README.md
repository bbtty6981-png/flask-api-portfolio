# Flask API Portfolio

このリポジトリは、Flask・Docker・AWS EC2 を使用して構築した  
**シンプルで拡張しやすいバックエンド API アプリケーション**です。

API 実装スキル・Docker コンテナ化・AWS EC2 へのデプロイ経験を  
案件応募時に示すためのポートフォリオとして作成しています。

---

## 📌 使用技術（Tech Stack）

- Python 3.10
- Flask
- Docker
- AWS EC2（Amazon Linux 2023）
- Git / GitHub

---

## 📁 フォルダ構成

flask-api-portfolio/
├── app.py
├── Dockerfile
├── requirements.txt
├── src/
│ ├── init.py
│ ├── routes/
│ │ ├── init.py
│ │ ├── sample.py
│ │ └── items.py
│ └── services/
│ ├── init.py
│ ├── item_service.py
│ └── sample_service.py
├── README.md
└── .gitignore

---

## 🚀 API エンドポイント一覧

### GET /sample/
テスト用の簡易エンドポイント。

GET http://<EC2のIP>:5001/sample/

---

### GET /items/
サンプルアイテムリストを返す API。

レスポンス例：

```json
[
  "apple",
  "banana"
]
🔧 ローカル起動方法（非 Docker）
pip install -r requirements.txt
python app.py
🐳 Docker ビルド＆実行
イメージのビルド
docker build -t flask-api .
コンテナ起動
docker run -d -p 5001:5001 flask-api
☁ AWS EC2 へのデプロイ
本アプリは AWS EC2 上で Docker コンテナとして運用しています。
EC2: Amazon Linux 2023
Docker にて Flask API を稼働
セキュリティグループ & iptables で 5001 番ポートを許可済み
🌐 公開 URL（動作中）
実際に動く API：
http://3.26.7.18:5001/items/
📌 ポートフォリオとしての目的
Flask を使った API 実装スキルを示す
Docker 化し EC2 上にデプロイできる技術を証明
GitHub 運用スキルを示すための実践プロジェクト
📬 作者
bbtty6981-png
https://github.com/bbtty6981-png

---

# 🔥 README.md の反映手順

EC2 上で：

cd ~/flask-api-portfolio
nano README.md

⬇ 上の内容を全部貼り付け  
⬇ 保存（Ctrl+O → Enter）  
⬇ 閉じる（Ctrl+X）

---

## GitHub へ反映

git add README.md
git commit -m "Add completed README for portfolio"
git push

