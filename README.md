# Compactador de Texturas para iRacing

Este aplicativo simples em Python serve para **reduzir o uso de VRAM no simulador iRacing**, compactando as texturas das pinturas dos carros adversários. Ele redimensiona as imagens `.TGA` usadas como pinturas dos carros para uma resolução menor (1024x1024 ou 512x512), diminuindo significativamente o consumo de memória de vídeo.

---

## Por que usar?

* **Economia de VRAM:** Jogos modernos consomem muita memória de vídeo com texturas em alta resolução, o que pode causar lentidão ou travamentos, especialmente em grids grandes.
* **Foco nas pinturas importantes:** O aplicativo permite definir IDs de pilotos (por exemplo, você e sua equipe) cujas pinturas **não serão modificadas**, garantindo que suas texturas continuem em alta qualidade.
* **Backup automático:** Pode criar backups dos arquivos originais antes da compactação, para restaurar caso deseje.
* **Interface gráfica amigável:** Fácil de usar, com seleção da pasta de pinturas, escolha da resolução, controle de backup e barra de progresso visual.

---

## Como funciona?

1. Você seleciona a pasta base onde ficam as pinturas do iRacing (normalmente em `Documents/iRacing/paint`).
2. Informa os IDs dos pilotos cujas pinturas devem ser preservadas (não compactadas).
3. Escolhe se deseja fazer backup dos arquivos originais e qual resolução deseja para as texturas compactadas.
4. Clica em "Iniciar Compactação".
5. O programa percorre todas as imagens `.TGA` dentro da pasta e suas subpastas, redimensionando todas exceto as que têm IDs preservados.
6. Exibe uma barra de progresso durante o processo e um resumo ao final.

---

## Benefícios

* **Melhora a performance** do iRacing em PCs com VRAM limitada.
* **Preserva a qualidade visual** dos pilotos mais importantes.
* **Evita modificações arriscadas** durante a execução do jogo, trabalhando apenas nos arquivos no disco.

---

## Tecnologias usadas

* Python 3
* Biblioteca Pillow para manipulação de imagens
* Tkinter para interface gráfica

---

## Como contribuir

Contribuições são bem-vindas! Abra issues, envie pull requests ou sugestões para melhorar a ferramenta.
