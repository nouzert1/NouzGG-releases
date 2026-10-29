# NouzGG

Overlay externo para Counter-Strike 2 — ESP, gatilho e painel.

**Baixe o `NouzGG.exe` na aba [Releases](../../releases/latest).**

## Como usar

1. Entre numa **partida** — o ESP não desenha no menu principal, porque não há mundo carregado.
2. Abra `NouzGG.exe` **como administrador**.
3. `INSERT` abre e fecha o painel.

Não há instalador e não há nada a configurar. É **um arquivo só** e ele é autossuficiente: sem
nenhum arquivo de config, abre no modo `legit`, que é o padrão e o mais seguro.

## Atalhos

| tecla | ação |
| --- | --- |
| `HOME` | liga / desliga o ESP |
| `INSERT` | abre / fecha o painel |
| `F1` | caixas |
| `F2` | barra de vida + HP |
| `F3` | distância |
| `F4` | snaplines |
| `F5` | ignorar companheiros de time |
| `END` | sai |

### Aperte `HOME` antes de usar a loja ou o menu do jogo

O ESP precisa ficar **acima** do jogo para ser visto. Mas uma janela acima do jogo é
consultada primeiro em cada clique — e isso deixava a **loja e o `ESC` do CS2 sem resposta**.

Aperte `HOME`: o ESP sai da tela e o jogo fica com o mouse. **O gatilho continua atirando** —
só o ESP sai da frente. Aperte de novo para ele voltar.

## Requisitos

| | |
| --- | --- |
| Sistema | Windows 10 ou 11, 64 bits |
| Jogo | Counter-Strike 2, aberto **em partida** |
| Permissão | executar como administrador |

## Se algo der errado

- **Nada aparece na tela** — confirme que você está numa partida. No menu principal não há o
  que desenhar, e isso é de propósito.
- **O `ESC` ou a loja não respondem** — aperte `HOME`.
- **Fecha sozinho ao abrir** — execute como administrador.
- **O antivírus reclama** — esperado num overlay que lê a memória de outro processo.

## Quando o CS2 atualizar

Uma atualização do jogo muda os endereços de memória, e o overlay para de desenhar **sem dar
nenhum erro**. Quando isso acontecer, este binário precisa ser recompilado — acompanhe a aba
**Releases** para a versão nova.

---

**Somente leitura.** O programa lê a memória do jogo e desenha por cima: sem injeção de DLL,
sem hook, sem driver, e sem escrever nada no processo do jogo.