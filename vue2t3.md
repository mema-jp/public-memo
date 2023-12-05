|  案  |  概要  |  手順  |
| ---- | ---- | ---- |
|  vue2-no-class  |  移行ビルを使用する  | ` npm i vue@next ` <br> ` npm i -f @vue/compat ` <br> ` npm i -D -f typescript @vue/compiler-sfc @vue/cli-service@latest ` <br> ` npm uninstall -f vue-template-compiler `  |
|  vue2-class1  |  移行ビルを使用する   | ` npm i vue@next ` <br> ` npm i -f @vue/compat ` <br> ` npm i -D -f typescript @vue/compiler-sfc @vue/cli-service@latest ` <br> ` npm uninstall -f vue-template-compiler ` <br> ` npm i -f vue-class-component@next ` <br> ` npm i -f vue-property-decorator@rc ` <br> Component → Options  |
|  vue2-class2 |  移行ビルを使用する   | ` npm i vue@next ` <br> ` npm i -f @vue/compat ` <br> ` npm i -D -f typescript @vue/compiler-sfc @vue/cli-service@latest ` <br> ` npm uninstall -f vue-template-compiler `  |
|  vue2-file-to-vue3  |  vue2のファイルをvue3のプロジェクトに移行  | ` npm i vue@next ` <br> ` npm i -f @vue/compat ` <br> ` npm i -D -f typescript @vue/compiler-sfc @vue/cli-service@latest ` <br> ` npm uninstall -f vue-template-compiler `  |



,利点,欠点
Git 子モジュール,- プロジェクト内で直接ソースコードを確認・編集可能<br>- 特定のコミットやブランチを選択し、バージョンを柔軟に制御<br>- 主プロジェクトと同じバージョン管理システムを共有し、統一的な管理が可能,- 複数のプロジェクトで使用する場合、各プロジェクトで個別にサブモジュールの設定が必要<br>- サブモジュールを手動で更新して最新バージョンを取得する必要がある<br>- サブモジュールを含むプロジェクトをクローンする際、クローン時間が長くなる
npm パッケージ,- npmを通じてインストールし、使用と更新のプロセスを簡素化<br>- npmのバージョン管理を利用し、異なるバージョンを管理<br>- パッケージが公開されていれば、コミュニティと共有可能,- npmパッケージの依存関係とバージョンの互換性問題を処理<br>- プロジェクト内で直接ソースコードを変更できない<br>- コンポーネントライブラリがプライベートの場合、費用が発生する可能性がある
