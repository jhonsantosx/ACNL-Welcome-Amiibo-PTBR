# Instalar a tradução

[English](GUIDE.en.md)

Use **Welcome amiibo USA**, Title ID `0004000000198E00`. O download contém a tradução, não o jogo. Consulte a versão e as limitações em [Releases](https://github.com/jhonsantosx/ACNL-Welcome-Amiibo-PTBR/releases).

## No Nintendo 3DS com Luma3DS

1. Tenha o jogo instalado e funcionando. A tradução não precisa ser instalada pelo FBI.
2. Baixe o ZIP `ACNL_Welcome_amiibo_PTBR_…_Luma.zip` nos anexos da release e extraia no computador.
3. Salve, feche o jogo e desligue o console antes de retirar o SD.
4. Copie a pasta **luma** do ZIP para a **raiz do SD**, mesclando com a pasta existente. Não apague a pasta luma inteira.
5. Confira a estrutura abaixo, ejete o cartão e coloque-o no console.
6. Segure **SELECT** enquanto liga o 3DS. Marque **Enable game patching** com **A** e use **START** para salvar e iniciar.
7. Abra o jogo normalmente pelo menu HOME.

```text
SD:/
└── luma/
    └── titles/
        └── 0004000000198E00/
            ├── locale.txt
            └── romfs/
                └── Script/
                    ├── Bbs/
                    ├── MailN/
                    ├── MailR/
                    ├── Str/
                    └── Talk/
```

Não deixe a estrutura dentro de uma pasta extra como `SD:/ACNL_PTBR/luma/` ou `SD:/luma/luma/`.

O `locale.txt` incluído contém **`USA EN`**. Ele seleciona o inglês, idioma-base substituído pelo PT-BR; mantenha esse conteúdo mesmo se o console estiver em português. O mecanismo de instalação é o [LayeredFS do Luma3DS](https://github.com/LumaTeam/Luma3DS/wiki/Optional-features).

## No Citra

1. Tenha sua cópia do jogo já funcionando no emulador.
2. Na lista de jogos, clique com o botão direito em **Welcome amiibo** e escolha **Abrir pasta de Mods**.
3. No ZIP, abra `luma/titles/0004000000198E00/` e copie **somente a pasta romfs** para a pasta de mods aberta pelo Citra.
4. Nas configurações do sistema emulado, use o idioma **English/Inglês**. O `locale.txt` é do Luma e não substitui essa configuração no Citra.
5. Feche e abra o jogo para carregar os arquivos novos.

O caminho deve terminar em `load/mods/0004000000198E00/romfs/Script/…`. No emulador, não coloque a árvore `luma/titles` dentro da pasta de mods.

## Se não aparecer em português

- Confira o **Title ID**, a pasta e o idioma-base.
- No console, confirme **Enable game patching**.
- Confira a versão do patch em `VERSAO.txt` no download.
- Uma fala isolada em inglês pode ser uma pendência da prévia; não significa necessariamente falha de instalação.
- Se persistir, [abra um relato](https://github.com/jhonsantosx/ACNL-Welcome-Amiibo-PTBR/issues/new/choose) com versão, plataforma e print. Se houver uma atualização oficial instalada, informe também.

## O que já foi testado?

Os arquivos passam por conferências de integridade, comandos e tamanho de texto. Isso não garante que todas as situações estejam corretas no jogo. A validação visual integral no console permanece pendente. Veja [STATUS](STATUS.md).
