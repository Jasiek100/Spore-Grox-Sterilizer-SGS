# Spore Grox Sterilizer (SGS) v1.0
**Created & Developed by Jasiek100**  
*Copyright © 2026 Jasiek100. All Rights Reserved.*

---

## ★ Overview
<p align="center">
  <img src="SPGS%208.11.2026.png" alt="Spore Grox Sterilizer Interface" width="750">
</p>
**Spore Grox Sterilizer (SGS)** is a standalone external tool for EA's *Spore* that autonomously neutralizes Grox star systems within a 20-parsec radius around the player ship.

Unlike traditional modding approaches, **SGS requires ZERO game modifications**:
- **NO DLL injection**
- **NO executable patching or modification of `SporeApp.exe`**
- **NO memory hooks or code caves**
- **100% clean vanilla save files** that load and play seamlessly on any computer without mods or scripts installed.

---

## ★ Key Features
1. **Automated Proximity Sterilization**:
   - Customizable sweep radius from **1 to 100 parsecs** directly in the GUI.
   - Rate-limited to **1 nearest system every 100 milliseconds** for rock-solid stability and zero flight stutter.
2. **Crash-Free Planetary Descent**:
   - Preserves all physical terrain seeds, water levels, atmospheres, oceans, and spice geysers by keeping internal `mKey` database identifiers untouched.
   - Converts planets back to pristine, natural wild worlds (Creature stage tech level 1, 0 UFO defenders, neutralized civilization vectors).
3. **Atomic Flight Engine Safety**:
   - Uses atomic memory transactions wrapped in `NtSuspendProcess` / `NtResumeProcess` to avoid race conditions during active space flight.
   - Automatically maintains Grox empire route topologies (`mNextStarTowardsHome`) and pins reference counts to permanently prevent use-after-free engine crashes.
   - Instantly redraws galaxy empire territory lines and removes red bubbles.
4. **Live In-Flight Telemetry**:
   - Live Player Ship Coordinates $(X, Y, Z)$.
   - Real-time remaining Grox star count.
   - Nearest Grox star name, exact distance, and relative directional vectors $(\Delta X, \Delta Y, \Delta Z)$ to make hunting remaining systems effortless.

---

## ★ How to Use
1. Launch **Spore** and enter the **Space Stage**.
2. Run **`SGS_V1.0.exe`** (or double-click `Spore_Grox_Sterilizer.bat`).
3. Fly your spaceship toward Grox territory.
4. Click **START STERILIZATION**.
5. As you fly through the galaxy, nearby Grox stars are automatically cured.
6. Save your game normally in Spore (`Esc` $\rightarrow$ `Save Game`). Your save file is 100% standard vanilla.

---

## ★ Authorship & Credits
- **Original Author & Reverse Engineer:** **Jasiek100**
- **Published:** November 2026
- **License:** GNU General Public License v3.0 (GPLv3)

### Notice on Plagiarism & Redistribution:
If you feature, review, or redistribute this software, prominent credit to **Jasiek100** must be maintained. Modification or removal of author watermarks, branding, or licenses is strictly prohibited under GPLv3.
