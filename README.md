# Como instalar/configurar/usar o `hardinfo` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos de como instalar/configurar/usar o `hardinfo` no `Linux Ubuntu`.

## _Abstract_

_In this document are contained the main commands to install/set up/use the `hardinfo` on `Linux Ubuntu`._

### Descrição

O termo "HardDisk" refere-se ao disco rígido, ou HDD (Hard Disk Drive), um dispositivo de armazenamento permanente usado em computadores e outros dispositivos eletrônicos. Ele consiste em discos magnéticos rotativos revestidos com material magnético, onde os dados são gravados por meio de cabeças de leitura/gravação. Os HDDs são amplamente utilizados devido à sua capacidade de armazenamento, custo mais baixo por gigabyte em comparação com SSDs (Solid State Drives), e são essenciais para o armazenamento de sistemas operacionais, aplicativos e arquivos pessoais em computadores tradicionais.

## 1. Como verificar o HD/SSD com o `hardinfo` no `Linux Ubuntu` [1]

Para configurar o `hardinfo`, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    



3. Para instalar o `HardInfo` no `Ubuntu`, você pode usar o terminal e executar os seguintes comandos. Instale o `HardInfo`: `sudo apt install hardinfo`

Depois de instalado, você pode executar o `HardInfo` através do terminal digitando `hardinfo` ou pode encontrá-lo no menu de aplicações do seu ambiente de `desktop`.

Isso irá instalar o `HardInfo` e você poderá usá-lo para visualizar informações detalhadas sobre o _hardware_ do seu sistema.

## Referências

[1] OPENAI. ***Instalar hardinfo no ubuntu:*** https://chat.openai.com/c/3aba3fd9-397f-4794-b8a9-ebd1c96ca826 (texto adaptado). Acessado em: 13/10/2023 09:28.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). Acessado em: 16/11/2023 14:25.

