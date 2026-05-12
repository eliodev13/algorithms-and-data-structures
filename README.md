# Algoritmi e Strutture Dati

Materiale di studio per l'esame di **Algoritmi e Strutture Dati** — Università degli Studi di Napoli "Parthenope".

Ogni argomento è trattato con pseudocodice (nella cartella `pseudocodice/`) e implementazione in C++ (nella cartella `implementazioni/`).

---

## Struttura della repository

```
.
├── teoria/                         # Appunti teorici
├── esercizi/                       # Esercizi per lo scritto
├── pseudocodice/                   # Pseudocodice degli algoritmi
│   ├── grafi/
│   ├── tabelle-hash/
│   ├── huffman/
│   ├── knapsack/
│   ├── lcs/
│   ├── memoizzazione/
│   ├── scheduling/
│   └── ordinamento/
└── implementazioni/                # Codice C++
    ├── grafi/
    │   ├── bfs/
    │   ├── dfs/
    │   ├── ordinamento-topologico/
    │   └── scc/
    ├── alberi-binari-ricerca/
    ├── alberi-rosso-nero/
    ├── tabelle-hash/
    ├── heap/
    ├── huffman/
    └── test/
```

---

## Contenuto per argomento

### Grafi — `pseudocodice/grafi/` · `implementazioni/grafi/`

| Algoritmo | Pseudocodice | Implementazione |
|-----------|-------------|-----------------|
| BFS (visita in ampiezza) | `bfs-visita.txt` | `bfs/BFS.cpp` |
| BFS — cammini minimi | `bfs-cammini-minimi.txt` | — |
| BFS — cicli e self-loop | `bfs-cicli-self-loop.txt` | — |
| BFS — nodi a distanza > K | `bfs-nodi-distanza-maggiore-k.txt` | — |
| DFS (visita in profondità) | `dfs-visita.txt` | `dfs/DFS.cpp` |
| DFS — componenti connesse | `dfs-componenti-connesse.txt` | — |
| DFS — cicli e self-loop | `dfs-cicli-self-loop.txt` | — |
| DFS — rilevamento cicli | `dfs-rilevamento-cicli.txt` | — |
| DFS — ciclo più lungo | `dfs-ciclo-piu-lungo.txt` | — |
| DFS — classificazione archi forward | `dfs-archi-forward.txt`, `dfs-lista-archi-forward.txt` | — |
| DFS — archi trasversali | `dfs-archi-trasversali.txt` | — |
| DFS — archi backward | `dfs-archi-backward.txt` | — |
| Dijkstra | `dijkstra.txt` | — |
| Bellman-Ford | `bellman-ford.txt` | — |
| Kruskal (MST) | `kruskal.txt` | — |
| Prim (MST) | `prim.txt` | — |
| MST — altezza, profondità, rango | `mst-altezza.txt`, `mst-profondita-massima.txt`, `mst-rango-minimo.txt`, `mst-rango-massimo.txt` | — |
| MST — arco minimo escluso | `mst-arco-minimo-escluso.txt` | — |
| MST — peso ciclo massimo | `peso-ciclo-massimo.md` | — |
| SCC — algoritmo di Kosaraju | `scc-kosaraju.txt` | `scc/SCC.cpp` |
| SCC — DFS su grafo trasposto | `scc-dfs-grafo-trasposto.txt` | — |
| Ciclo hamiltoniano | `ciclo-hamiltoniano.txt` | — |
| Ordinamento topologico | — | `ordinamento-topologico/ordinamento-topologico.cpp` |
| Implementazione completa (BFS+DFS+SCC+Topo) | — | `grafi-completo.cpp` |
| Guide e promemoria | `promemoria-bfs-dfs.md`, `componenti-connesse.md` | — |

### Strutture Dati ad Albero

| Struttura | Pseudocodice | Implementazione |
|-----------|-------------|-----------------|
| Albero binario di ricerca (ABR) | — | `alberi-binari-ricerca/ABR.cpp` |
| ABR — varianti personali e di studio | — | `ABR-mio.cpp`, `ABR-luca.cpp`, `ABR-rocco.cpp` |
| Albero rosso-nero (RB) | — | `alberi-rosso-nero/RB.cpp` |
| Max-Heap | — | `heap/max-heap.cpp` |
| Min-Heap | — | `heap/min-heap.cpp` |

### Tabelle Hash — `pseudocodice/tabelle-hash/` · `implementazioni/tabelle-hash/`

| Tecnica | Pseudocodice | Implementazione |
|---------|-------------|-----------------|
| Concatenamento (chaining) | `tabelle-hash.txt` | `Hash-concatenamento.cpp` |
| Indirizzamento aperto (linear probing) | `tabelle-hash.txt` | `Hash-indirizzamento-aperto.cpp` |

### Algoritmi Greedy

| Algoritmo | Pseudocodice | Implementazione |
|-----------|-------------|-----------------|
| Huffman | `pseudocodice/huffman/huffman.txt` | `implementazioni/huffman/huffman.cpp` |
| Knapsack frazionario | `pseudocodice/knapsack/knapsack-frazionario.txt` | — |
| SJF — Shortest Job First | `pseudocodice/scheduling/sjf-schedulazione.txt` | — |

### Programmazione Dinamica

| Algoritmo | Pseudocodice |
|-----------|-------------|
| Knapsack 0/1 | `pseudocodice/knapsack/knapsack-01.txt` |
| LCS — lunghezza | `pseudocodice/lcs/lcs-lunghezza.txt` |
| LCS — con ricostruzione del percorso | `pseudocodice/lcs/lcs-ricostruzione.txt` |
| LCS — con memoizzazione | `pseudocodice/lcs/lcs-memoizzazione.txt` |
| Catena di montaggio | `pseudocodice/scheduling/catena-di-montaggio.txt` |
| Merge Sort | `pseudocodice/ordinamento/merge-sort.txt` |

### Memoizzazione — `pseudocodice/memoizzazione/`

- `memoizzazione-sottostruttura-ottima.txt` — struttura generale con tabella di memoizzazione
- `calcola-numero.txt` — formula ricorsiva G(n) = G(n-1)+G(n-2)+G(n-3)
- `quadrato-di-n.txt` — esempio base

---

## Teoria — `teoria/`

| File | Argomento |
|------|-----------|
| `automi-a-stati-finiti.md` | DFA — Automi a stati finiti deterministici |
| `macchina-di-turing.md` | Macchina di Turing |
| `complessita-NP-e-classeP.md` | Classi P e NP, riduzioni polinomiali |
| `problemi-NP-completi.md` | Problemi NP-completi principali |
| `problemi-indecidibili.md` | Problemi indecidibili e tesi di Church-Turing |
| `regole-generiche.md` | Regole e proprietà generali |

---

## Esercizi — `esercizi/`

- `esercizi-scritto-1.txt` / `esercizi-scritto-2.txt` / `esercizi-scritto-3.txt` — esercizi per lo scritto d'esame
- `esercitazioni.txt` — esercitazioni guidate

---

## Note sulle implementazioni C++

Molti file esistono in varianti multiple:
- **`[nome].cpp`** — implementazione di riferimento
- **`[nome]-mio.cpp`** — variante personale sviluppata durante lo studio
- **`[nome]-file.cpp`** — variante che carica i dati da file
- **`[nome]-luca.cpp` / `[nome]-rocco.cpp`** — varianti di compagni di corso
