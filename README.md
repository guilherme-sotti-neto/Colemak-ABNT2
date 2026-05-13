# Colemak Para ABNT2 (PT-BR) Linux
Fiz esse layout pois não encontrei para Português, nem para Linux, e muito menos ABNT2.

No bloco de notas:
- Usei o layout padrão ABNT2;
- Mudei a posição das letras.

No arquivo [QWYÇ TROCADOS Portuguese (Brazil, Colemak).xkb](https://github.com/guilherme-sotti-neto/Colemak-ABNT2/blob/main/QWYÇ%20TROCADOS%20Portuguese%20(Brazil,%20Colemak).xkb) troquei a posição do Q e W, e Y e Ç para facilitar a digitação.
## Como Implemantar

- Vá ao diretório de arquivos de símbolos ```/usr/share/X11/xkb/symbols```;
- Edite o arquivo ```br``` existente com permissão de administrador;
- Adicione a nova variante de layout no final do arquivo (escolha entre [Portuguese (Brazil, Colemak).xkb](https://github.com/guilherme-sotti-neto/Colemak-ABNT2/blob/main/Portuguese%20(Brazil%2C%20Colemak).xkb) e [QWYÇ TROCADOS Portuguese (Brazil, Colemak).xkb](https://github.com/guilherme-sotti-neto/Colemak-ABNT2/blob/main/QWYÇ%20TROCADOS%20Portuguese%20(Brazil,%20Colemak).xkb)) e salve;
- Edite o registro XML ```/usr/share/X11/xkb/rules/evdev.xml``` com permissão de administrador. Dentro do bloco ```<variantList>``` do português adicione a variante:
```
<variant>
  <configItem>
    <name>colemak</name>
    <description>Portuguese (Brazil, Colemak)</description>
  </configItem> 
</variant>
```
- Limpe o cache pelo Terminal ```sudo rm -rf /var/lib/xkb/*```;
- Adicione a fonte de entrada ```Portuguese (Brazil, Colemak)``` nas configurações do teclado.

Layout:

<img width="795" height="395" alt="Captura de tela de 2026-05-13 14-59-05" src="https://github.com/user-attachments/assets/942f21be-03b6-41f5-aa48-de10b8fee41f" />

Shift pressionado:

<img width="795" height="395" alt="Captura de tela de 2026-05-13 14-59-08" src="https://github.com/user-attachments/assets/4e73f5c7-3711-4a3c-a369-cc424b787624" />

AltGr pressionado:

<img width="795" height="395" alt="Captura de tela de 2026-05-13 14-59-10" src="https://github.com/user-attachments/assets/a5fe6698-e091-4507-a4a1-5861b6929ba4" />

Shift+AltGr pressionados:

<img width="795" height="395" alt="Captura de tela de 2026-05-13 14-59-13" src="https://github.com/user-attachments/assets/0318ec76-5b7f-496b-b5e8-a3120d317159" />
