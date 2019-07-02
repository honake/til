# compy
- 競技プログラミング用のコードスニペット集
- Snippets for Competitive Programming

# snippets
- UnionFind.py
  - グループ分けを木構造で管理するデータ構造
  - 同じグループに属する＝同じ木に属するという木構造でグループ分け
    - 要素xと要素yが同じグループに属するかどうかを判定したい
      - 要素xの根と要素yの根が同じならば同じグループ，要素xの根と要素yの根が同じでないならば異なるグループにあることが分かる
    - 要素xと要素yが同じグループに属する場合，要素xの属するグループと要素yの属するグループに併合
  - parentには以下を格納
    - 小の場合（正値）は親のインデックス
    - 親の場合（負値）はその集合のサイズ
- Deque.py
  - Pythonリストはスタック利用はOKだがキューは遅い
    - たとえば`pop(0)`はO(n); 先頭要素を削除→配列を1つずつ前にズラす
  - → colletions.dequeを利用
- Dijkstra.py
  - 辺の重みが非負数の場合の単一始点最短経路問題を解くための最良優先探索
  - 重みに負数がある場合はベルマンフォード法
