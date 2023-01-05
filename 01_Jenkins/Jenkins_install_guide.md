# Dockerを使ったJenkinsサーバ構築
1. Docker Desktopの導入
    * 公式サイトからインストール
        * https://www.docker.com/products/docker-desktop/
2. Jenkins Dockerイメージのダウンロード
    * Docker Desktopが起動した状態でWSLにて以下を実行
        ```
        docker pull jenkins/jenkins
        ```
3. Jenkinsの起動
    * WSLにて以下を実行
        ```
        docker run -p 8080:8080 -p 50000:50000 jenkins/jenkins
        ```
        * 次回、起動時からは docker startで起動

* 参考
    * https://yoshikiito.net/blog/archives/2330/
    * https://qiita.com/legitwhiz/items/e6ac1f5a94f09ff2bb1d

# WindowsにJenkinsサーバ構築
    * https://peloproject.com/%E3%83%84%E3%83%BC%E3%83%AB/%E3%80%90jenkins%E3%80%91windows%E3%81%ABjenkins%E3%82%92%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%99%E3%82%8B%E6%89%8B%E9%A0%86/

# LinuxにJenkinsサーバ構築
    * https://www.jenkins.io/doc/book/installing/linux/