# GDB2SHP
Conversão de formatos: GDB (ESRI File Geodatabase) em SHP (ESRI Shapefile)

Exemplos de chamadas de funções (batch):
```batch
REM Export de uma shapefile ou diretoria de shapefiles para o formato GDB

REM Export de um conjunto de shapefiles (diretoria) para uma GDB (criacao da GDB)
CALL "C:\cpc_apps\shp2gdb\shp2gdb.pyc" "D:\temp\test" "D:\temp\mapping_file_shp2gdb.csv" "D:\temp\test.gdb"

REM Export de uma shapefile para uma GDB (criacao da GDB)
CALL "C:\cpc_apps\shp2gdb\shp2gdb.pyc" "D:\temp\test\L_Ponte.shp" "D:\temp\mapping_file_shp2gdb.csv" "D:\temp\test.gdb"
```
