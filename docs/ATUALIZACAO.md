# Atualizar sem perder sua cidade

[English](GUIDE.en.md#updating)

**Você não precisa reinstalar o jogo, apagar o save ou começar novamente.** O patch fica em uma pasta separada e é carregado quando o jogo inicia.

## Atualização habitual no 3DS

1. Leia as notas da nova release.
2. Salve, feche o jogo e desligue o console.
3. Extraia o novo ZIP no computador.
4. Copie a pasta **luma** para a raiz do SD, mesclando as pastas e aceitando substituir os arquivos deste jogo.
5. Ejete o cartão, recoloque no console e abra o jogo.

Não apague `Nintendo 3DS`, não desinstale o título e não remova a pasta `luma` inteira.

## Quando houver remoção de arquivos

As notas da release devem informar se o conjunto de arquivos mudou. Para evitar arquivos antigos sobrando, faça uma substituição completa **somente da tradução**:

1. Guarde no computador uma cópia de `SD:/luma/titles/0004000000198E00/romfs`.
2. Remova apenas essa pasta `romfs` do SD.
3. Copie a nova pasta `romfs` inteira para o mesmo lugar, junto do `locale.txt` fornecido.

Esse caminho contém os arquivos do patch, não a cidade salva. Se você usa outros mods nesse mesmo caminho, não misture pacotes sem conferir a compatibilidade.

## No Citra

Com o jogo fechado, substitua a pasta `romfs` dentro da pasta de mods de Welcome amiibo. Preserve os diretórios de save do emulador. Abra o jogo novamente.

## Voltar à versão anterior ou desativar

Restaure a pasta de tradução que você guardou. Para desativar, mova somente a pasta do patch para fora do caminho usado pelo Luma ou pelo Citra. Não é preciso apagar o save.

Atualização **do patch PT-BR** é diferente de atualização oficial **do jogo**. Este guia trata do patch.

Referência: [LayeredFS do Luma3DS](https://github.com/LumaTeam/Luma3DS/wiki/Optional-features).
