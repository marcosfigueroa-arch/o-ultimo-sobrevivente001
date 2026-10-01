# 🔥 O Último Sobrevivente

Jogo de tiro em primeira pessoa (FPS) 3D que roda direto no navegador, no computador ou no celular. Sobreviva a 15 ondas de zumbis, enfrente o chefe final, suba de patente e colecione personagens com habilidades diferentes.

**Jogar:** https://gabrieljacintooliveira-glitch.github.io/o-ultimo-sobrevivente/

---

## 🎮 Como jogar

Escolha um modo no lobby, sobreviva às ondas e gaste seus pontos na **loja de cartas** que abre entre uma onda e outra. Nas ondas **5, 10 e 15** aparecem zumbis armados. A onda 15 termina com o **chefe final** (35.000 de vida).

### Controles no computador

| Tecla | Ação |
|---|---|
| W A S D | Mover |
| Mouse | Mirar |
| Clique esquerdo | Atirar (segure para atirar automático) |
| R | Recarregar |
| Espaço | Pular |
| Shift | Correr (gasta stamina) |
| Q | Habilidade do personagem |
| Esc | Pausar |

### Controles no celular

Jogue com o celular na horizontal.

- **Joystick à esquerda:** andar
- **Deslizar o dedo na metade direita da tela:** mirar
- **Botões:** FOGO, PULO, R (recarregar), CORRER e Q (habilidade)

---

## ✨ Recursos

- **Lobby estilo Free Fire** com personagem 3D que gira (arraste para girar), brasas animadas e vagas de esquadrão.
- **Online com amigos** em salas de até 4 jogadores, com código de 5 letras.
- **Patentes:** 22 níveis, de Bronze I até Lendário, com XP salvo no navegador.
- **Personagens com habilidades** e **Royale** (roletas de Ouro e de Diamante).
- **Loja de cartas** com upgrades entre as ondas.
- **Efeitos:** sons gerados por código, headshot com dano extra, números de dano flutuantes, tela vermelha ao ser atingido e regeneração lenta de vida.

---

## 🧑 Personagens

| Personagem | Raridade | Passiva | Habilidade (Q) |
|---|---|---|---|
| 🪖 Soldado | Comum (grátis) | +20 de vida máxima | Cura 40 de vida (30s) |
| ⚡ Velocista | Comum (grátis) | +15% de velocidade | Investida para frente (8s) |
| 🎯 Atirador | Raro | +20% de dano, headshot x3 | Dano dobrado por 6s (25s) |
| 💉 Médica | Rara | Regeneração 3x mais rápida | Cura 70 de vida (35s) |
| 🛡️ Tanque | Épico | +70 de vida máxima, -8% de velocidade | Invencível por 4s (40s) |
| 💣 Demolidor | Épico | +10% de dano | Explosão em área com 220 de dano (20s) |

---

## 🎰 Royale e moedas

| Roleta | Custo | Chances |
|---|---|---|
| Ouro Royale | 300 🪙 | 18% personagem raro, 5% épico, o resto vira XP ou diamantes |
| Diamante Royale | 60 💎 | 35% personagem raro, 25% épico, o resto vira XP ou diamantes |

Só saem personagens que você ainda não tem. Se já tiver todos, o valor gasto volta.

**Como ganhar moedas jogando:**

- Zumbi morto: 5 de ouro
- Chefe: 200 de ouro
- Onda completa: 50 de ouro e 3 diamantes
- Vitória: 500 de ouro e 50 diamantes
- Subir de patente: 10 diamantes

Todo jogador começa com 600 de ouro e 120 diamantes. As moedas são só do jogo, sem compra com dinheiro de verdade.

---

## 🎖️ Patentes e XP

| Ação | XP |
|---|---|
| Matar um zumbi | 10 |
| Matar com headshot | 15 |
| Matar o chefe | 500 |
| Completar uma onda | 40 + 10 por número da onda |
| Vencer o jogo | 1000 |

Escada: Bronze I-III, Prata I-III, Ouro I-IV, Platina I-IV, Diamante I-IV, Heroico, Mestre, Grão-Mestre e Lendário.

---

## 🌐 Jogar online

1. Um jogador clica em **Criar sala online** e passa o código de 5 letras aos amigos.
2. Os amigos digitam o código em **Entrar na sala**.
3. O anfitrião clica em **Iniciar partida**.

A conexão é direta entre os jogadores (WebRTC, via [PeerJS](https://peerjs.com/)), então não precisa de servidor próprio.

**Limitações atuais:**

- Os jogadores se veem e disputam um placar, mas **cada um enfrenta os próprios zumbis**. Os inimigos não são compartilhados.
- O PeerJS usa um servidor público gratuito para o primeiro contato, que às vezes falha. Se o código não conectar, crie uma sala nova.
- Algumas redes de celular ou de empresa bloqueiam conexões diretas.

---

## 💾 Progresso salvo

Patente, XP, moedas, personagens e personagem escolhido ficam salvos no **navegador do aparelho** (`localStorage`). Eles não passam de um aparelho para outro e são apagados se os dados do navegador forem limpos.

---

## 🚀 Publicar no GitHub Pages

1. Coloque o arquivo `index.html` na raiz do repositório.
2. Em **Settings → Pages**, escolha a branch `main` e a pasta `/ (root)`.
3. Aguarde alguns minutos e acesse o link do site.

Não há etapa de instalação nem de build. O jogo é um único arquivo HTML.

---

## 🛠️ Tecnologia

- HTML, CSS e JavaScript em um único arquivo
- [Three.js](https://threejs.org/) r128 para os gráficos 3D
- Web Audio API para os sons
- PeerJS para o modo online
- `localStorage` para o progresso

---

## 🗺️ Ideias para o futuro

- Co-op com zumbis compartilhados entre os jogadores
- Modo PvP
- Personagens aparecendo no corpo dos jogadores online
- Mira assistida no celular
- Mais armas, mapas e cartas
