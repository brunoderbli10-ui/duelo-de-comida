# Duelo de Comida

Jogo de duelo em pixel art feito com HTML5 Canvas e JavaScript puro (sem bibliotecas, sem imagens externas — tudo desenhado em tempo real).

Dois jogadores se enfrentam à distância: a comida voa sozinha, então o negócio é **desviar, defletir com o escudo e usar o especial do seu personagem na hora certa**.

## Como jogar

Abra o `index.html` no navegador (duplo clique já funciona).

1. Tela inicial → qualquer tecla abre a **seleção de personagens**.
2. Cada jogador escolhe o seu lutador e confirma.
3. `Enter` começa a partida (ou quando os dois confirmarem).
4. `Esc` volta ao menu.

### Controles

| Ação | P1 (WASD) | P2 (setas) |
|------|-----------|------------|
| Bandeira do país | `A` (segurar) | `←` (segurar) |
| Defletir (escudo) | `D` | `→` |
| Pular | `W` | `↑` |
| Especial | `S` | `↓` |

- **Bandeira erguida por 3s = +1 escudo** (até 5). Enquanto ela está levantada você não pode usar o escudo nem arremessar comida.
- O escudo **devolve** a comida em vez de destruí-la, e só gasta carga quando realmente deflete algo.
- **Especial custa 3 escudos** e tem um aviso de ~0,6s antes de acertar.

## Personagens e especiais

| Personagem | Bandeira | Arremessa | Especial |
|------------|----------|-----------|----------|
| George Washington | EUA | hambúrguer | **Chá** — bule no céu deixa o rival confuso por 3s (comandos trocados) |
| Napoleão Bonaparte | França | croissant | **Urso polar** — urso batendo continência no céu congela o rival por 3s |
| Che Guevara | Cuba | charuto | **Guerrilha** — companheiros aparecem e roubam 2 escudos do rival |
| Josef Stalin | URSS | vodka | **Tanque T-34** — 25 de dano, ignora escudo |
| Elon Musk | SpaceX | foguetinho | **Foguete** — 18 de dano e o rival perde 2 escudos |
| Margaret Thatcher | Reino Unido | xícara de chá | **Dama de Ferro** — invulnerável por 3s (armadura + coroa de ferro) |

## Detalhes técnicos

- Um único arquivo `index.html`, sem dependências.
- Sprites, bandeiras, comidas e efeitos são grades de pixels desenhadas no canvas.
- Áudio gerado por Web Audio API (trilha e efeitos), com botão **SOM ON/OFF**.
- Botões **MENU** e **SOM** no rodapé, e `M` para mutar.
