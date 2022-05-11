◎Linux Photorealistic Game MOD
Created by takamitsu_h

これは、vkBasaltとReShade FX Shadersを使って、Linux版Steamで動作しているゲームやゲームエミュレーターで動作しているゲームの画質を大幅に向上し、フォトリアルに仕上げる物です。

◇関連記事
https://www.vsrx.work/article/487851526.html

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
   - cas
ReShade FX Shaders
   - MXAO.fx
   - AmbientLight.fx
   - Colourfulness.fx
   - FakeHDR.fx
   - Curves.fx
   - Clarity.fx
   - DPX.fx
   - MagicBloom.fx
   - FineSharp.fx
   - ReflectiveBumpMapping.fx
   - AdaptiveFog.fx
   - FilmicPass.fx
   - FilmGrain.fx
   - LiftGammaGain.fx
   - HSLShift.fx
   - CinematicDOF.fx

◇超美麗化の効果が高いおすすめゲームタイトルとツール
- Linux版Steam
  Dead Or Alive 5 Last Round
  Biohazard HD remaster
  アスタブリード
  NiGHTS
  巫剣神威控
- PPSSPP