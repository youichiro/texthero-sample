# texthero-sample

## setup

```bash
$ git clone https://github.com/youichiro/texthero-sample.git
$ cd texthero-sample
$ pip install -r requirements.txt
```

mecabを使えるようにする

```bash
$ brew install mecab
$ brew install mecab-ipadic
```

日本語のプロットで文字化けしないようにフォントをダウンロードする

```bash
$ cd fonts
$ wget https://noto-website-2.storage.googleapis.com/pkgs/NotoSansCJKjp-hinted.zip
unzip NotoSansCJKjp-hinted.zip -d NotoSansCJKJP
$ cd ..
```

ストップワードを用意する

```bash
$ cd dicts
$ wget http://svn.sourceforge.jp/svnroot/slothlib/CSharp/Version1/SlothLib/NLP/Filter/StopWord/word/Japanese.txt -O stopwords.txt
$ cd ..
```

livedoorニュースコーパスを取得する

```bash
$ wget https://gist.githubusercontent.com/nxdataka/48a27b2e1c3f029e7f25e66dba4b6dde/raw/75b56c34869c6b290cdb54a0925f34baeace021a/ldn2csv.py
$ python ldn2csv.py -o data/livedoornews.csv
```

notebookを開く

```bash
$ jupyter notebook notebooks/texthero.ipynb
```
