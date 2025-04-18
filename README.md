# navi cheats

インタラクティブなチートシートツール [navi](https://github.com/denisidoro/navi) のためのチートシート集です。

## navi インストール

### Arch Linux

```shellsession
$ sudo pacman -Syu navi
```

### Mac

```shellsession
$ brew install navi
```

## チートシートの登録

`~/.local/share/navi/cheats` に拡張子 `.cheat` のファイルを含むディレクトリを配置することで `navi` がチートシートを認識します。

ここでは、ローカルにクローンしたリポジトリへのシンボリックリンクを作成します。

```shellsession
$ git clone git@github.com:tacbooon/navi-cheats.git ~/repos/navi-cheats
$ mkdir -p ~/.local/share/navi/cheats
$ ln -s ~/repos/navi-cheats ~/.local/share/navi/cheats/tacbooon__navi-cheats
```

## チートシートの更新

`navi` にはチートシートを更新する機能がありません。別途 `.cheat` ファイルを更新する手段を用意する必要があります。

前述の手段でチートシートを更新した場合、ローカルリポジトリを更新することで `navi` に最新のチートシートを反映できます。

```shellsession
$ cd ~/repos/navi-cheats
$ git pull --rebase
```
