**Creación de un ambiente Conda**  

```shell
conda update -n base -c defaults conda
conda create -n biomonitoreo-participativo-datos
conda activate biomonitoreo-participativo-datos
conda install -c conda-forge gdal
conda deactivate
```

**Capas geoespaciales**
```shell
conda activate biomonitoreo-participativo-datos
```

```shell
# Áreas silvestres protegidas (ASP)
ogr2ogr -t_srs EPSG:4326 -makevalid asp.geojson WFS:"http://geos1pne.sirefor.go.cr/wfs?" "PNE:areas_silvestres_protegidas"
```

```shell
conda deactivate
```
