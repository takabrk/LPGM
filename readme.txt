◎Linux Photorealistic Game MOD
Created by takamitsu_h

これは、vkBasalt+ReShade FX Shaders+qUINTを使って、Linux版Steam上で動作するゲームやゲームエミュレーター上で動くゲームの画質を大幅に向上し、フォトリアルに仕上げる物です。

◇関連記事
https://www.vsrx.work/article/487851526.html

◇使用するツールとシェーダ
vkBasalt - Linux用のポストプロセッシングツール。WindowsのReShadeのような機能を持っており、グラフィックスAPIにはVulkanが使われています。
https://github.com/DadSchoorse/vkBasalt

Ubuntuでのインストール方法は、以下の通りです。
$ sudo apt install vkbasalt

ReShade FX Shaders - ReShade用のシェーダ集。vkBasaltでも、ほとんどのシェーダーが使えます。
https://github.com/crosire/reshade-shaders

qUINT - ReShade用のシェーダ集。vkBasaltで使用可能です。
https://github.com/martymcmodding/qUINT

◇使い方
1.Steam(Linux version) Photoreal setをダウンロード
2.homeディレクトリの.configディレクトリにvkBasaltディレクトリを新規作成する
3.作成したvkBasaltフォルダに、解凍したファイルを入れる
4.Steamを起動し、各ゲームのプロパティの起動オプションに以下を追加すると使えます。

ENABLE_VKBASALT=1 %command%

◇Linux上での動作ディレクトリ構成

/---home
      |-<user>
          |---.config
                |-vkBasalt
                    |---vkBasalt.conf
                    |---reshade-shaders-master

◇使用しているシェーダ
vkBasalt
   - fxaa
ReShade FX Shaders
   - AmbientLight.fx
   - FakeHDR.fx
   - Curves.fx
   - DPX.fx
   - MagicBloom.fx
   - FineSharp.fx
   - ReflectiveBumpMapping.fx
   - AdaptiveFog.fx
   - CinematicDOF.fx
   - FineSharp.fx
   - qUINT_sharp.fx

◇超美麗化の効果が高いおすすめゲームタイトルとツール
- Linux版Steam
  Dead Or Alive 5 Last Round
  Biohazard HD remaster
  アスタブリード
  NiGHTS
  巫剣神威控
- PPSSPP