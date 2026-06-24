# PrivateSpotify — Git e Inventário

## Regra principal

O Git guarda documentação, scripts e inventários. Não guarda ficheiros de música.

## Ficheiros importantes

- inventory/My Spotify Library.txt: lista original do Spotify
- inventory/navidrome_current_files.txt: músicas já existentes no Raspberry Pi/Navidrome

## Biblioteca real

As músicas reais ficam no Raspberry Pi em:

/srv/music

## Antes de adicionar música nova

1. Atualizar inventory/navidrome_current_files.txt a partir do Raspberry Pi.
2. Verificar se a música já existe nesse inventário.
3. Só depois processar metadata, copiar para /srv/music e fazer scan no Navidrome.

## Regra Git

Nunca adicionar ficheiros .m4a, .mp4, .mp3, .flac, .wav ou .ogg ao Git.
