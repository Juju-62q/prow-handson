# Prow入門

## 目的
* Prowのようなk8sベースのCI/CDについて、全体をなんとなく理解して、いざCI/CDが壊れたらなんとなく見る場所がわかるくらい。
* 開発側のエンジニアにとって、Prow自体とProwを使った理想の開発体験を知ってもらう。
* CI/CD構築側のエンジニアにとって、Prowについてゼロ知識から短時間で理解して、使うか判断できる状態。
* 最初と最後の状態
    * 最初
        * Prowってなに？おいしいの？
        * kubernetesどどう関係あるの？
        * 何となく概要はわかってるけど、時間取って勉強するの面倒くさい、誰かわかりやすく説明して。
    * 最後
        * 勉強会終わったらもう導入する。明日出社したら導入する。
        * ProwもしくはProwみたいなのでGithub周りの自動化したい、生産性上げたい。

## ターゲット
* ProwやCI/CDについて普段からそんなにキャッチアップしていない人
* 開発をメインでやりたいからCI/CDについて本腰をいれて勉強する気はない人
* なんとなく全体がふわっとわかればいいなという人
* CI/CDを構築する側より使う側のエンジニア

### 非ターゲット
* 日頃からCI/CDの選定や構築に勤しんでいる人