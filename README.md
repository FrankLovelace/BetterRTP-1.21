"Forked from BetterRTP by SuperRonanCraft."
# 🌌 BetterRTP - FrankLovelace Fork

Este es un **Fork publico** de [BetterRTP](https://github.com/SuperRonanCraft/BetterRTP) optimizado para **Minecraft 1.21+** y **Java 21**.

El objetivo de este fork es mantener la funcionalidad principal de RTP (Random Teleport) eliminando dependencias obsoletas ("Bloatware") que impiden la compilación en entornos modernos.

---

##  Cambios Técnicos (Changelog)

###  Actualizaciones
*   **Java Target:** Actualizado de Java 8 a **Java 21** (Requerido para Paper 1.20.5+).
*   **Paper API:** Actualizada a `1.21.1-R0.1-SNAPSHOT`.
*   **Lombok:** Actualizado a `1.18.36` para compatibilidad con el compilador de Java 21.
*   **Repositorios:** Se migraron repositorios HTTP inseguros a HTTPS y se añadió `CodeMC`.

###  Integraciones Eliminadas (Podadas)
Para lograr una compilación limpia, se eliminaron las integraciones con los siguientes plugins (cuyas dependencias estaban rotas, deprecadas o eran privadas):

1.  **Residence:** (Dependencia local faltante).
2.  **FactionsBridge:** (Dependencia local faltante).
3.  **MinePlots:** (Repositorio caído).
4.  **UltimateClaims:** (Errores de compilación).

*Nota: El plugin sigue funcionando perfectamente con WorldGuard, GriefPrevention y protecciones estándar.*

---

##  Cómo Compilar

Necesitas **Maven** y **JDK 21** instalados.

```bash
mvn clean package -U