# 第6回 解答

## 演習

<!-- [tool call] の行は、表示された行をそのまま貼り付けてください。終わらなかった STEP は、空欄のままでかまいません。 -->

- STEP 1 のツールの名前：search_glossary
- STEP 2 の [tool call]：glossary_search_glossary({'query': '3レベル'})
- STEP 3 の [tool call]：fetch_fetch({'url': 'https://modelcontextprotocol.io/'})
- STEP 4 の [tool call]：aws_aws___search_documentation({'topics': ['general'], 'search_phrase': 'Amazon S3 versioning overview'})
- 気づき・疑問：設定ファイルに書き足しただけで、ローカル実行とリモート実行を切り替えることができることがわかった。
また、ローカル実行に比べてリモート実行はコンテキストの消費量が大きくなる。
STEP2で読んでいる検索クエリでは質問で「３レベル」と「3レベル」を別と扱っており、LLMであっても質問の質で結果が変わるとわかった。

## 宿題

<!-- 基礎・実装・発展のどれか1つに取り組めば完了です。 -->

- 取り組んだレベル：基礎
- やったこと：get_lecture_summaryをMCPサーバーに公開した
- 結果：lecture02の内容を読み取り、質問に対して回答を返すことができた
- 気づき・疑問：mcp_server.pyに1行書き足すだけで、新しいツールを公開することができることがわかった。
