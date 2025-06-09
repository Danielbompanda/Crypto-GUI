# Script de Criptografia com Zenity e GPG

Este script Python permite proteger arquivos com senha (criptografar) e abrir arquivos protegidos (descriptografar) usando uma interface gráfica simples.

---

## Requisitos

Antes de usar, você precisa ter instalado no seu sistema:

- Python 3
- Zenity (exibe as janelas gráficas)
- GPG (ferramenta de criptografia)
- O pacote Python `python-gnupg`

---

## Como instalar as dependências

### Para Debian, Ubuntu e derivados:

```bash
sudo apt update
sudo apt install python3 python3-pip gnupg zenity -y
pip3 install python-gnupg
```

### Para Fedora:

```bash
sudo dnf install python3 python3-pip gnupg2 zenity -y
pip3 install python-gnupg
```

### Para Arch Linux / Manjaro:

```bash
sudo pacman -Syu python python-pip gnupg zenity --noconfirm
pip install --user python-gnupg
```

---

## Como usar

1. Salve o script como `criptografia.py`.

2. Abra o terminal na pasta onde o arquivo está.

3. Rode o programa com:

```bash
python3 criptografia.py
```

4. Vai aparecer uma janela com três opções:

- **Criptografar arquivo**: Escolha o arquivo para proteger com senha.  
  Depois digite a senha. O arquivo criptografado será criado com extensão `.gpg`.

- **Descriptografar arquivo**: Escolha o arquivo `.gpg` para abrir.  
  Digite a senha usada para proteger. O arquivo original será restaurado.

- **Sair**: Fecha o programa.

---

## Atenção

- Guarde bem a senha usada para criptografar. Sem ela, não tem como abrir o arquivo depois.  
- Esse script foi feito para sistemas Linux com Zenity e GPG instalados.  
- No Windows, você pode usar dentro do WSL (Linux no Windows) ou pedir uma versão para Windows.

---

Se precisar de ajuda para instalar ou usar, só avisar!

---

## Licença

Sinta-se livre para usar e modificar este script para seus projetos pessoais ou profissionais.
