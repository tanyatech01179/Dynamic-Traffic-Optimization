# METR-LA Dataset Setup

This project uses the METR-LA traffic dataset to analyze traffic patterns and perform dynamic graph-based route optimization.

## Dataset Files

Download the following three files:

1. **METR-LA Traffic Data (`metr-la.h5`)**  
   [Download metr-la.h5](https://huggingface.co/datasets/MintBruce/SkyTraffic/resolve/main/metr-la.h5)

2. **Sensor Locations (`graph_sensor_locations.csv`)**  
   [Download graph_sensor_locations.csv](https://raw.githubusercontent.com/liyaguang/DCRNN/master/data/sensor_graph/graph_sensor_locations.csv)

3. **Sensor Distance Matrix (`distances_la_2012.csv`)**  
   [Download distances_la_2012.csv](https://raw.githubusercontent.com/liyaguang/DCRNN/master/data/sensor_graph/distances_la_2012.csv)

## Where to Place the Files

After downloading, place all three files inside this `data` directory.

The expected structure is:

```text
data/
├── metr-la.h5
├── graph_sensor_locations.csv
├── distances_la_2012.csv
└── README.md
```

## Important Note

The METR-LA HDF5 file is relatively large and is excluded from this GitHub repository through `.gitignore`.

Download it separately before running the notebook.

The notebook also supports a deterministic synthetic dataset fallback when the real dataset is unavailable.