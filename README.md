# Blogger_HTML_tag_cleaner
Blogger_ぺージhtml内部のtagのエラー,重複を検出、ある程度自動修正するスクリプトファイル。このスクリプトにてhtmlを修正した後,更にhtmlエディタでインデント状態などを微調整。Google Canvas 作成。
This script file detects and corrects errors and duplicate tags within the HTML of a Blogger page. After correcting the HTML with this script, further fine-tuning can be done with an HTML editor.

#背景
;Blogger のページ生成機能にて大量の<div>,<span>,タグが挿入され、編集により閉じ忘れなどエラーが生じ,表示が崩れる場合の修正
;2025～2026年代に急速に普及したAIチャット生成文を貼り付ける場合,やはり大量のhtmlタグやCSSが,編集により依存関係が破損したり閉じ忘れなどエラーが生じ、表示が崩れる場合の修正
;ページのデータ量の圧縮
;
#使い方
;Blogger編集画面の「html」画面から、ページのhtmlコード全体をコピーし、ツールのウィンドゥにペーストして実行。
;
#既知の問題
;まれにColorアトリビュートが消去,又は,無効となり,文字列が透明（色無し）になる部分が出る場合がある
;CSSの状態によってはBlogger側の自動整形機能により,内容が部分的に削除されてしまう（「作成ビュー」リロードにて確認が必要）
;<div>,</div>タグなどが全角に変換されて残る場合がある。
;「URLエンコード日本語化」(日本語可読化)選択機能は正常に機能しない場合がある。また、影響でCSSが破損して表示が崩れる場合がある(リロードして確認が必要)
;コードの「コピー」(copy)ボタンの機能は,バッファ容量約1MBに制限(Windows11実行環境の場合)され,コード後半は無視される。1MBを越える場合は,「ダウンロード」(download)機能を使用して下さい。
;
#direct_link:  https://bluestackson.github.io/Blogger_HTML_tag_cleaner/blogger_html_tester.html
; 
#Script
<div style="width: 100%; overflow: hidden; border-radius: 8px; border: 1px solid #334155;">
  <iframe 
    src="https://bluestackson.github.io/Blogger_HTML_tag_cleaner/blogger_html_tester.html" 
    style="width: 100%; height: 600px; border: none;" 
    title="Blogger HTML クリーナー"
    loading="lazy">
  </iframe>
</div>
;   
#拡張Script
<div style="width: 100%; border-radius: 8px; border: 1px solid #334155; background: #0f172a; overflow: hidden; font-family: sans-serif;">
  <!-- 別タブで大きく開くボタン -->
  <div style="padding: 8px 12px; background: #1e293b; text-align: right; border-bottom: 1px solid #334155;">
    <a href="https://bluestackson.github.io/Blogger_HTML_tag_cleaner/blogger_html_tester.html" 
       target="_blank" 
       rel="noopener noreferrer" 
       style="color: #38bdf8; font-size: 11px; text-decoration: none; font-weight: bold;">
      ↗ 全画面でツールを開く
    </a>
  </div>
  
  <!-- ツール本体 iframe -->
  <iframe 
    src="https://bluestackson.github.io/Blogger_HTML_tag_cleaner/blogger_html_tester.html" 
    style="width: 100%; height: 500px; border: none; display: block;" 
    title="Blogger HTML クリーナー"
    loading="lazy">
  </iframe>
</div>
