# ブランチを分ける

まとまった変更などがある場合や編集途中で更新されてほしくない場合，blanchを変えることで履歴を保存しつつ
実際のページは更新されないようにできます．

現在，`.github/workflows/hugo.yaml`にて`main`branchがpushされた時に
GitHub Actionsでデプロイが行われるようになっています．

ある程度の記事が書き上がり，本格的に運用するようになり次第，
mainブランチへのpushを一旦ロックする予定です．

これは，意図しない変更やミスによる`main`ブランチへのpushを防ぐためです．  
手癖で`git push origin main`しても変更への承認がないとpushされないようになります．

この時の更新の仕方は後述する**Pull Requestを作る**で言及します．

# branchを使う
変更した，あるいはこれから変更するものを別のbranchで扱いたい場合について

※`commit`はbranchを変更するまで待ってください．

変更を別のbranchとして作成するためには，
`git checkout -b <作成するbranch名>`としてブランチを作成し，そのブランチに移動します．

ここで，`main`ブランチで行っていた時と同様に`git add`や`git commit`などを行い，
`git push origin <branch名>`とすることでそのbranchでGitHubに記録することができます．

# Pull Requestを作る
// TODO
- PRの作り方
- レビューについて
- mainブランチへの統合は1承認以上とかにする
  - 自分で承認でもアリ
  - 見てもらいたい時は共有