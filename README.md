# AttFirmware_StLinkV2-to-Blackmagic

Obs: Tudo isso feito no Windows.

Primeiro será necessário que você possua dois StLink V2, um será seu novo BlackMagic e o outro servirá para gravar o firmware no primeiro.

Pinos a serem conectados:

St Link v2

> SWDIO --> SWDIO

> GND --> GND

> SWCLK --> SWCLK

> 3.3V --> 3.3V

- Devemos baixar e instalar o Software STM32CubeProgrammer;

- Baixe os dois arquivos que estão neste repositório;

- No CubeProgrammer, clique no ícone a esquerda (Erasing and Programming);

- Selecione o caminho do primeiro arquivo (blackmagic_dfu-stlink.bin);

- Coloque o endereço como: 0x08000000 e clique em Start Programmer;

![image](https://user-images.githubusercontent.com/47569587/135146021-a1c3442f-965d-4644-b8a5-b9c6be62f12b.png)

- Depois desse passo, selecione novamente o caminho, agora do outro arquivo (blackmagic-stlink.bin);

- Coloque o endereço como: 0x08002000 e clique em Start Programmer;

![image](https://user-images.githubusercontent.com/47569587/135147562-9dce4ebf-29dc-4cef-afe3-99e2ff6f781c.png)

- Pronto! Seu BlackMagic está pronto.
