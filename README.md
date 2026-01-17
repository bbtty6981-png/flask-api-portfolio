# 🚀 Flask API Portfolio

本リポジトリは、副業案件・実務未経験応募向けに作成したシンプルな Flask API ポートフォリオです。  
Docker 化・API 設計・AWS EC2 デプロイまで一通りの基礎技術力を示す目的で作成しています。

---

## 📌 Features（できること）

- Flask を利用した REST API
- ルーティング層 / サービス層の分離による実務的コード構成
- Docker によるコンテナ実行
- AWS EC2 上でのデプロイ実績
- 公開 API をそのまま確認可能

---

## 📁 Project Structure（構成）

flask-api-portfolio/  
├── app.py  
├── src/  
│   ├── routes/  
│   │   └── items.py  
│   └── services/  
│       └── item_service.py  
├── requirements.txt  
├── Dockerfile  
└── docker-compose.yml  

---

## 🧪 API Specification（API 仕様）

### GET /items/
サンプルのアイテム一覧を返す API。

Response example:
[
  "apple",
  "banana"
]

---

## 🐳 Run with Docker（ローカル実行）

1. イメージをビルド & 起動  
docker-compose up --build

2. 確認  
http://localhost:5001/items/

---

## ☁️ Deployment（AWS EC2 で動作中）

- OS: Amazon Linux 2023  
- Docker + docker-compose で実行  
- セキュリティグループで 5001 を開放  
- 公開中 API（例）  
http://<EC2 Public IP>:5001/items/

---

## 🎯 Purpose（この成果物の目的）

- Web/API 系副業案件の応募時に提出  
- Flask / API / Docker / EC2 を扱える基礎力を示す  
- ポートフォリオとして企業へ共有しやすい

---

## 📄 License

MIT License
