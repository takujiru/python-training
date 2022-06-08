# ゼロからの Python 入門講座

https://www.python.jp/train/index.html

を順に実施

- [ばえる Python](https://www.python.jp/train/experience/next-sample.html)
  - 【問題】requests が no modules
    - ローカル環境には requests が pip install されていなかった
    - pip install requests で解決
    - [ソースコード](../src/introduction-to-python-from-zero/next-sample.py)
  - 【問題】まだ requests が no modules
    - pip と python が異なるものを見ていた（ので、pip で install しても python では使えない）
      - pip => pyenv
      - python => 非 pyenv
    - pyenv を使うことにする
      - pyenv install -l
      - pyenv install 3.10.5
      - pyenv local 3.10.5
      - pyenv --version
  - 【問題】まだ requests が no modules
    - py -m pip install --upgrade pip した時に別の場所の pip を見ていた
    - py コマンドが python コマンドのエイリアスになっていなかった
    - python -m pip install --upgrade pip で解決
  - 【問題】PIL が no modules
    - pip show PIL で Package(s) not found を確認
    - ✕ pip install PIL
    - pip install pillow
    - 解決
