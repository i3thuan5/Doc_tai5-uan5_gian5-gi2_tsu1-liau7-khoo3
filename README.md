# 臺灣言語資料庫

這是一個用Django撰寫的資料庫套件，幫助人們快速建立一個語料庫。

它包含語料庫常用表格以及匯入匯出的API，能夠儲存純文字，影音，以及聽打資料，不論是台語/客語/族語都適用。

除了當語料庫，它很適合搭配臺灣言語服務，那是一個台語/客語/族語parser，提供語音辨識和語音合成。

### 安裝

```bash
sudo apt-get install -y python3 python-virtualenv g++ python3-dev zlib1g-dev libbz2-dev liblzma-dev libboost-all-dev libyaml-dev libav-tools libmp3lame0 libavcodec-extra-* libpq-dev python3-dev postgresql postgresql-contrib # pgsql
virtualenv --python=python3 venv; source venv/bin/activate
pip install --upgrade pip
pip install tai5-uan5_gian5-gi2_tsu1-liau7-khoo3
```

安裝後，初始化資料庫：

```bash
python manage.py migrate
python manage.py 顯示資料數量

外語有0筆，影音有0筆，文本有0筆，聽拍有0筆
```

完成。想看如何從頭開始安裝，請看安裝步驟。

### 注意！

每次在終端機開新分頁後，都必須重新載入虛擬的python環境：

```bash
source venv/bin/activate
```

```bash
# 載入成功後會顯示(venv)在帳號前。
(venv) YOUR_ACCOUNT $ ...
```

### 我想幫忙

請看[開發](開發.md)

### License

[MIT](License)

