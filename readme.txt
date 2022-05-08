◎Steam(Linux version) Photoreal set

これは、vkBasaltとReShade FX Shadersを使って、Linux版Steamで動作しているゲームの画質を大幅に向上し、フォトリアルに仕上げる物です。

◇使用するツールとシェーダ
vkBasalt - Linux用のポストプロセッシングツール。WindowsのReShadeのような機能を持っており、グラフィックスAPIにはVulkanが使われています。
https://github.com/DadSchoorse/vkBasalt

Ubuntuでのインストール方法は、以下の通りです。
$ sudo apt install vkbasalt

ReShade FX Shaders - ReShade用のシェーダ集。vkBasaltでも、ほとんどのシェーダーが使えます。
https://github.com/crosire/reshade-shaders

◇使い方
1.Steam(Linux version) Photoreal setをダウンロード
2.homeディレクトリの.configディレクトリにvkBasaltディレクトリを新規作成する
3.作成したvkBasaltフォルダに、解凍したファイルを入れる
4.Steamを起動し、各ゲームのプロパティの起動オプションに以下を追加すると使えます。

ENABLE_VKBASALT=1 %command%

◇ディレクトリ構成

/---home
      |-<user>
          |---.config
                |---vkBasalt.conf
                |---reshade-shaders-master