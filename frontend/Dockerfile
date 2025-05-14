# ベースイメージ
FROM node:20

# 作業ディレクトリの設定
WORKDIR /app

# package.json と package-lock.json を先にコピー
COPY package*.json ./

# 依存パッケージのインストール
RUN npm install

# 残りのアプリケーションファイルをコピー
COPY . .

# React 開発サーバーが使用するポートを公開
EXPOSE 3000

# 開発サーバーを起動
CMD ["npm", "start"]