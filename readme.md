## Чтобы заработал VIM как надо

```
cd ~
apt install vim
apt install npm
npm install -g n
n stable
curl -sL install-node.now.sh/lts | bash
```
[Как поставить clang](https://clangd.llvm.org/installation)
```
apt-get install clangd-15
```
### Тут возможно надо еще вторая строчка но у меня заработало без 2 строчки

### Копируем конфиг из файла себе

```
vim ~/.vimrc
```
 
[Что бы были доступны плагины](https://github.com/junegunn/vim-plug)
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
### Выполняем в vim
```
:PlugInstall
:source %
```
### Для автодополнения
```
:CocInstall coc-clangd
```
