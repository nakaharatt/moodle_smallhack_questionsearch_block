# moodle_smallhack_questionsearch_block
Moodle 4.5の問題バンクにおいてテキストブロックを利用したJavaScriptによる問題検索機能を追加するコード

## 設定手順
1. （任意）エディタプレファレンスでエディタをプレインテキストに変更する 
2. 検索機能を追加したい問題バンクに移動し、編集モードをオンにする
3. ブロックの追加よりテキストブロックを追加
4. script.htmlのコードをペーストして保存

## 使い方
1. すべて表示するをクリックして問題をすべて表示する（すでに検索対象が表示されているのであれば不要）
2. 検索文字列を入力して検索ボタンをクリック

## 注意点
1. 問題バンクに4000問以上登録されている場合は、4000にハードコードされているqperpageの値を適宜修正してください。
2. 検索対象は現在表示されている問題の問題名、問題テキスト、作成者、修正 byです。
3. すべてにチェックする機能には対応させているつもりですが、削除等の操作には十分気をつけてください。
4. すべて表示する機能は、問題バンクのフィルタに依存します。すべて表示させたいカテゴリ（コーストップなど）を選んだ状態でご利用ください。
5. すべて表示を解除して、ページング状態に戻するには、さらに..から問題バンクを開くなどqperpageパラメータをなくせば戻るはずです。それでも戻らない場合は「カラムをリセットする」ボタンをクリックしてみてください。

## Adding a JavaScript-Powered Question Search Feature to the Moodle 4.5 Question Bank

This guide will walk you through adding a search feature to your Moodle 4.5 question bank using a text block and some JavaScript code.

### Setup Instructions
1. **(Optional) Change Editor Preference:** For easier code pasting, you might want to switch your editor preference to plain text. You can usually find this option in your user profile settings.
2. **Navigate to the Question Bank:** Go to the question bank where you want to add the search feature. Turn editing mode on for this question bank.
3. **Add a Text Block:** From the "Add a block" menu, choose "Text block."
4. **Paste the Code:** Copy the code from the `script.html` file and paste it into the text block you just added. Save the block.

### How to Use the Search
1. **Display All Questions:** Click the "Show all" button to display all questions in the bank. This step is only necessary if the questions you want to search are not currently visible.
2. **Enter Your Search:** Type your search terms into the provided search field. Click the "Search" button to initiate the search.

### Important Notes
1. **Handling Large Question Banks:** If your question bank contains more than 4000 questions, you'll need to adjust the `qperpage` value in the JavaScript code. This value is currently set to 4000. Increase it as needed to accommodate your larger question bank.
2. **Search Scope:** The search function will search within the currently displayed questions, looking for matches in the question name, question text, author, and "modified by" fields.
3. **Careful with Bulk Actions:** While a "Select all" checkbox is included, please exercise extreme caution when performing bulk actions like deleting questions. Double-check your selections to avoid unintended consequences.
4. **"Show All" Functionality:** The "Show all" function relies on the question bank's filters. To ensure all questions are displayed, select the appropriate category (e.g., the course top level) before using the "Show all" button.
5. **Returning to Paged View:** To exit the "Show all" view and return to the paginated view of the question bank, you can either open the question bank from a different location (which removes the `qperpage` parameter from the URL) or click the "Reset columns" button.
