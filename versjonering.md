# Regler for versjonering av kjernen
Versjonering av kjernen skal følge Semantic Versioning (SemVer): https://semver.org/spec/v2.0.0.html
__NB! Enhver som skal lage ny versjon av kjernen MÅ lese og forstå denne først.__

## Versjonsnavn release
Format: x.y.z  
Eksempel: 8.0.0

## Versjonsnavn pre-release
Format: x.y.z-\<PRERELEASENAME>\<BUILDNUMBER>  
Eksempler:
- Alpha-versjon: 8.0.0-alpha12
- Beta-versjon: 8.0.0-beta12
- Release Candidate: 8.0.0-rc12
- Branch: 8.0.0-innsyn12

PRERELEASENAME settes i Mqr4.build.xml i <PrereleaseName> tagen. Når denne er satt lages versjonsnavnet som en pre-release og blir oppfattet av NuGet som en pre-release pakke. BUILDNUMBER oppdateres automatisk ved bygg.

## Beskrivelse av versjonstall
- x: Major version – Ny funksjonalitet har blitt introdusert. Registeret må gjøre minst én kode-/konfigurasjonsendring for å kunne ta i bruk denne versjonen (ikke bakoverkombatibel)
- y: Minor version – Ny funksjonalitet har blitt introdusert. Registeret kan oppgradere til denne versjonen uten å gjøre noen endringer i kode / konfigurasjon (bakoverkompatibel)
- z: Patch – Bug fiks, ingen ny funksjonalitet. Registre kan oppgradere til denne versjonen uten å gjøre noen endringer i kode  / konfigurasjon (bakoverkompatibel)
