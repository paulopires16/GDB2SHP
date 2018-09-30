# GDB2SHP
Conversão de formatos: GDB (ESRI File Geodatabase) em SHP (ESRI Shapefile)

Exemplos de chamadas de funções (batch):
```batch
REM Export de uma featureClass, lista de featureClass's ou featureDataset (separados por virgula) de uma GDB para o formato SHP

REM  exporta tudo
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\test.gdb" "D:\temp\test_shp"

REM  exporta apenas a FC: L_Ponte
CALL PYTHON "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\test.gdb" "D:\temp\test_shp" "L_Ponte"

REM  exporta todas as FC's da FDS topo
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\test.gdb" "D:\temp\test_shp" "topo"

REM  exporta todas as FC's da FDS WGS84 e a FC tpn
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\test.gdb" "D:\temp\test_shp" "WGS84,tpn"

REM  exporta as FC's feature1,feature2 e todas as FC's da FDS featuredataset1
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\test.gdb" "D:\temp\test_shp" "feature1,feature2,featuredataset1"
```
