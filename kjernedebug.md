# Debugging av kjernekode
Skriptet som kobler kjernekode til registerkode slik at man kan kjøre debug på den er f.o.m v8 flyttet fra hvert enkelt register og til kjernen for å sentralisere vedlikehold av det.

Skriptet ligger under Tools katalogen.  
Navn: DebugCoreLocally.bat  
parameter: PATH_TIL_REGISTER

Eks.:
```
DebugCoreLocally.bat "c:\Kildekode\Mrs\Tonsille"
```

## Husk
For å debugge siste versjon av kjernekode følg disse stegene
1. Kompiler kjerneløsningen
2. Kjør DebugCoreLocally.bat
3. Kompiler registerløsningen

