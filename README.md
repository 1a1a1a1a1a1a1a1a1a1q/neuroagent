# NEUROAGENT

Biologische Intelligenz → KI-Architektur

Analysiert das Drosophila (Fruchtfliege) Connectome, extrahiert biologische Prinzipien der Informationsverarbeitung und generiert daraus neue KI-Architekturen.

## Was macht das?

1. **Connectome laden** — Strukturell akkurater Subset des FlyWire Drosophila-Connectomes (~13.500 Neuronen, 10 Gehirnregionen)
2. **KI-Agent forscht autonom** — Ein LLM analysiert das Gehirn mit 8 Analyse-Tools (Hub-Erkennung, Community Detection, Motif-Suche, Signal-Simulation, ...)
3. **Prinzipien extrahieren** — Biologische Designprinzipien identifizieren (Sparse Connectivity, Laterale Inhibition, Hub-Neuronen, E/I-Balance)
4. **Architektur generieren** — PyTorch-Module die diese Prinzipien implementieren (Drop-in für Transformer)

## Schnellstart (RunPod)

```bash
# Repo klonen
git clone https://github.com/1a1a1a1a1a1a1a1a1a1q/neuroagent.git
cd neuroagent

# Dependencies
pip install -r requirements.txt

# Notebook starten
jupyter notebook neuroagent.ipynb
```

Die erste Code-Zelle im Notebook installiert Ollama und lädt Dolphin (uncensored) automatisch.

## GPU-Bedarf

| Modell | VRAM | GPUs (A100 80GB) |
|--------|------|-------------------|
| Dolphin Llama 3.1 405B (uncensored) | ~400GB | 8x A100 |
| Dolphin Llama 3.1 70B (uncensored) | ~140GB | 2x A100 |

## Analyse-Tools

| Tool | Beschreibung |
|------|-------------|
| `find_hubs` | Hub-Neuronen finden (PageRank, Betweenness, Degree) |
| `detect_communities` | Funktionale Cluster (Louvain) |
| `trace_signal` | Signalverfolgung durch das Netzwerk |
| `analyze_region` | Detailanalyse einer Gehirnregion |
| `find_motifs` | Netzwerk-Motifs (Feedforward/Feedback Loops) |
| `simulate_activation` | Spreading-Activation-Simulation |
| `compare_to_artificial` | Vergleich Bio vs. Transformer/CNN/RNN |
| `find_pathways` | Stärkste Pfade zwischen Regionen |

## Lizenz

MIT
