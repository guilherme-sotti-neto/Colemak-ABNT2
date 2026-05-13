# Colemak Para ABNT2 (PT-BR)
Fiz esse layout pois não encontrei para Português, nem para Linux, e muito menos ABNT2.

No bloco de notas:
- Usei o layout padrão ABNT2;
- Mudei a posição das letras.

## Como Implemantar

- Vá ao diretório de arquivos de símbolos ```/usr/share/X11/xkb/symbols```
- Edite o arquivo "br" existente com permissão de administrador
- Adicione a nova variante de layout no final do arquivo (escolha entre [Portuguese (Brazil, Colemak).xkb](https://github.com/guilherme-sotti-neto/Colemak-ABNT2/blob/main/Portuguese%20(Brazil%2C%20Colemak).xkb) e [QW TROCADOS Portuguese (Brazil, Colemak).xkb](https://github.com/guilherme-sotti-neto/Colemak-ABNT2/blob/main/QW%20TROCADOS%20Portuguese%20(Brazil,%20Colemak).xkb)) e salve;
- Edite o registro XML ```/usr/share/X11/xkb/rules/evdev.xml``` com permissão de administrador. Dentro do bloco ```<variantList>``` do português adicione a variante:
```
<variant>
  <configItem>
    <name>colemak</name>
    <description>Portuguese (Brazil, Colemak)</description>
  </configItem> 
</variant>
```
- Limpe o cache pelo Terminal ```sudo rm -rf /var/lib/xkb/*```
- Adicione a fonte de entrada "Portuguese (Brazil, Colemak)" nas configurações do teclado.

Layout:

<img width="812" height="406" alt="image" src="https://github.com/user-attachments/assets/80e6a7c7-ee77-42a3-a964-8ba555a9d238" />

Shift pressionado:

<img width="812" height="406" alt="image" src="https://github.com/user-attachments/assets/2e537c45-fa3c-4cea-9774-856e01810fa8" />

AltGr pressionado:

<img width="812" height="406" alt="image" src="https://github.com/user-attachments/assets/f115a129-2712-4a4e-9f2e-b8071fd904a2" />

Shift+AltGr pressionados:

<img width="812" height="406" alt="image" src="https://github.com/user-attachments/assets/2fd00068-5993-47ad-afeb-27e340d011b3" />



