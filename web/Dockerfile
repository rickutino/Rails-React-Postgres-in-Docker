# ベースイメージの作成
FROM node:12.17
# コンテナ内で作業するディレクトリを指定
RUN mkdir /web

WORKDIR /web
# package.jsonとyarn.lockを/usr/src/appにコピー
COPY ["package.json", "yarn.lock", "./"]
# パッケージをインストール
RUN yarn install
# ファイルを全部作業用ディレクトリにコピー
COPY . .