# GDB2SHP
Conversão de formatos: GDB (ESRI File Geodatabase) em SHP (ESRI Shapefile)

Exemplos de chamadas de funções (batch):
```batch
REM Export de uma featureClass, lista de featureClass's ou featureDataset (separados por virgula) de uma GDB para o formato SHP
REM seguem exemplos, basta retirar o 'rem' para a linha funcionar:

REM  exporta tudo
REM CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\250_top.gdb" "D:\temp\250_shp"

REM  exporta apenas a FC: A_Albufeira
CALL PYTHON "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\250_top.gdb" "D:\temp\250_shp" "L_Ponte_larga_de_betao_em_via"

REM  exporta todas as FC's da FDS toponimia
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\250_top.gdb" "D:\temp\250_shp" "toponimia"

REM  exporta todas as FC's da FDS WGS84_Mil e a FC tpn_Export (pre-validacao)
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\250_top.gdb" "D:\temp\250_shp" "WGS84_Mil,tpn_Export"

REM  exporta as FC's A_Albufeira,A_Azenha e todas as FC's da FDS toponimia
CALL "C:\cpc_apps\gdb2shp\gdb2shp.pyc" "D:\temp\250_top.gdb" "D:\temp\250_shp" "A_Albufeira,A_Azenha,toponimia"
```
