# Doom Chaves
Mod para o DOOM 2 baseado na franquia El Chavo del Ocho. | Mod for DOOM 2 based on franchise El Chavo del Ocho.  
Criado em 2014 quando eu tinha 15 anos. Atualizado a partir de 2020. | Created back in 2014 when I was 15. Updated back in 2020.  
Usa o formato DOOM 2 UDMF. | Uses DOOM 2 UDMF format.  
Necessário usar o lights.pk3 | Expects lights.pk3

### Veja o mod em ação no YouTube: | Watch the mod in action on YouTube:
[![Veja o mod em ação no YouTube, Watch the mod in action on YouTube](https://img.youtube.com/vi/fmqVgwJOd34/0.jpg)](https://youtu.be/fmqVgwJOd34)



# Como jogar/instalar o mod | How to play/install the mod
Tenha certeza de que está usando [GZDoom](https://zdoom.org/downloads) e que você tem uma cópia de Doom2.wad (precisa ser comprado na steam o Doom 2). | Make sure to use [GZDoom](https://zdoom.org/downloads) and have a copy of Doom2.wad (distribution of this one is illegal).  
Clique e arraste chaves.pk3 em cima de gzdoom.exe. | Click and drag chaves.pk3 on top of gzdoom.exe.  
Marque a opção Extra Graphics - Lights para fazer o GZDoom carregar lights.pk3, se não o mod ficará muito escuro em partes. | Make sure to check the checkbox that says Extra Graphics - Lights in order to load lights.pk3 inside GZDoom. The game gets too dark without it.

## Software utilizado | Software used:
### SLADE 3.2.1

Permite editar arquivos como texturas. | Allows for file editing such as textures.

### Ultimate Doom Builder R4015 (64-bit)

Cria mapas. Também uso para mexer nos scripts, apesar de ser possível usar o SLADE para isso também. Porém o UDB compila na hora de salvar o arquivo, e é mais prático. | Creates maps. I personally use it to script as well, even though SLADE can do it also, because UDB will compile every time you save.

# Coisas a fazer | Things that need to be done:
[Clique aqui para ver a lista de coisas a fazer | Trello board](https://trello.com/b/zAKgRyzS/doom-chaves)

# Arquivos | Files
DECORATE.TXT - Definição de Atores, inclui armas, monstros e informações do player. | Actor definition, includes weapons, monsters, and player info.  
GAMEINFO.TXT - Informação usada pelo GZDoom para bootar o jogo corretamente. | Information used by GZDoom to boot up the game correctly.  
SBARINFO.TXT - Faz a HUD do jogo. | Draws the HUD in the game.  
SNDINFO.TXT - Atrela arquivos de sons a nomes de variáveis. | Binds sound files to a variable name.  
SNDSEQ.TXT - Sons usados para portas e plataformas, ou em scripts. | Sounds to be used for doors and platforms or in scripts.[^1]  
MODELDEF.TXT - Definição dos modelos 3D (exportados em formato md3 e png para as texturas), somente funciona com OpenGL. Atualmente os únicos modelos 3D no mod são coisas que seriam complexas demais para serem feitas em sprite. | Definition for 3D models (exported in md3 format and png for textures), only work with OpenGL. Currently the only 3D models are objects in the map that seemed to complex to be achieved in 2D.  
LOCKDEFS.TXT - Definição das fechaduras, qual chave abre elas e qual mensagem é exibida na tela. | Definition for literal locks in the game, which key opens them and what message is exibited onscreen.[^2]  
MAPINFO.TXT - Informações relacionadas ao jogo, como qual playerclass o jogador vai usar, quais músicas usar onde, quais cores usar no GZDoom quando ele abre, se o jogador pode agachar ou não, e informações sobre os mapas, além de definições básicas dos mesmos. | Game related info, such as what playerclass the player will use, what songs to use, what colors to use, can the player crouch or not, and also information about the maps the player will go through as well, and basic definitions on those maps.[^3]  
ANIMDEFS.TXT - Definições de animação, como quantos ticks cada imagem vai ser exibida, atualmente usado somente nas televisões ligadas no mod. | Animation definitions, such as how many ticks each picture will display, currently only used to display switched on TV screens.  
TEXTURES - Arquivo que mapeia todas as texturas. | This file maps all textures.  
/flats/ - Pasta contendo texturas de chão ou teto, para exibir corretamente, o Slade precisa ter o Doom2.wad configurado como recurso base. | Folder containing all textures related to floor or ceilings. In order to display properly, Slade needs to be configured to have Doom2.wad as it's base resource.  
/graphics/ - Pasta contendo gráficos da tela principal e o texto. | Folder containing main screen graphics and text.  
/music/ - Contém arquivos de música, suporta MP3 mas fica pesado no tamanho do mod. | Contains music files. It supports MP3, but it's heavy on the filesize.  
/patches/ - Texturas usadas nas paredes, o skybox está aqui também. | Textures used for the walls. The skybox is here too.  
/sounds/ - Efeitos sonoros. | Sound effects.  
/sprites/ - Sprites para as coisas dentro do jogo. | Sprites for in-game things.  
/sprites/models/ - Imagens PNG vazias para os modelos 3D. Não lembro porque isso existe. | Empty PNGs for the 3D models. Not exactly sure why these exist anymore.  

## /maps/
map01.wad - Arquivos Wad são como pastas e a ordem dos arquivos dentro importa! Esse arquivo contém: | Wad files are archives and the order inside these files matter! This file contains:

MAP01 - Arquivo do mapa em sí, as linhas representam setores (como salas ou telhados "falsos" usando portais), e posição de coisas. Pode ser editado abrindo diretamente no UDB. Não recomendo abrir o UDB pelo Slade, tive alguns bugs assim, é melhor abrir diretamente. | File for the actual map itself, it's lines which represents sectors (such as rooms or the illusory rooftops made using portals), and things placement. Can be edited in UDB, I personally don't recommend opening UDB through Slade because it causes glitches, better to open it directly.  
TEXTMAP - Definição de todos os objetos do mapa. Automaticamente editado pelo UDB. | Definition of all objects in the map. Automatically edited by UDB.  
BEHAVIOR - Arquivo que contém os scripts em forma compilada. O UDB compila automaticamente usando acc.exe. | Lump that contains a map's scripts in compiled form. UDB will recompile these using acc.exe automatically.[^4]  
DIALOGUE - Usado para criar diálogo, não usado nesse mod. | Used for dialogue such as in Strife. Unused here. [Exemplo | Example](https://youtu.be/WjxJbo9jHFo?t=259)  
ZNODES - Criado automaticamente pelo UDB para o formato UDMF. | Built automatically by UDB for UDMF format.  
SCRIPTS - Scripts do mapa, é compilado toda vez que salvo no UDB, precisa ser compilado manualmente no Slade. Substitui o arquivo BEHAVIOR. | Map scripts, need to be recompiled after editing in Slade, will be recompiled automatically in UDB after each save, and will replace BEHAVIOR when you do so.  
ENDMAP - Arquivo que representa o final da pasta com 0 bytes. | 0 byte file that just represents the end of the archive.

# Agradecimentos especiais para: | Special thanks to:
freshlycutgrass & Rockstar Games (GTA 2 explosion effects)  
Agent ME (general Doom modding help)  
Cris140 (general sound related help and creator of AI Seu Madruga's voice)  
phantombeta (general Doom modding help)  
Agent_Ash (general Doom modding help)  
Beck (Beta tester & sprite artist)  
Aleksandro Junior (Beta tester 2014 version)  
ID Software  
...rest of DOOM (and by extent ZDoom) community

# Descrição original | Original description (in pt-BR)
**O que é?**

Doom Chaves é um mod para o jogo Doom, criado por mim em 2014, quando eu estava nos meus 15 anos. Na época, devido a falta de conhecimento, e outros compromissos, eu acabei abandonando o mod em um estado extremamente inicial. Depois de tantos anos, eu acabei lembrando que ele existia, e recomecei a trabalhar nele. 

**Ainda não entendi que porcaria é essa...**

Você deve se lembrar do jogo Doom, febre nos anos 90. O que você provavelmente não deve saber é que existe uma comunidade que modifica o jogo até hoje, criando coisas que seriam inimagináveis em um jogo dessa época. Doom Chaves pega esse clássico jogo e adiciona características do Chaves no jogo.

Referências | References
[^1]: [SNDSEQ](https://zdoom.org/wiki/SNDSEQ)
[^2]: [LOCKDEFS](https://zdoom.org/wiki/LOCKDEFS)
[^3]: [MAPINFO](https://zdoom.org/wiki/MAPINFO)
[^4]: [BEHAVIOR](https://zdoom.org/wiki/BEHAVIOR)  
