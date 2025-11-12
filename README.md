# CHIRP Radio Programming Documentation

## Introduction
This repository serves as a backup of my progress with CHIRP and radio programming experiences.

## Resources Used
I paid for access to [RadioReference.com](https://www.radioreference.com/) ($15.00) to query their database. While I only queried local results initially, I plan to expand this. Note: Many sites require monthly subscriptions for information that arguably should be freely available or donation-based, considering the already significant cost of equipment.

## Equipment/Images

### Kenwood TK-862G-1  (Default)
- [Default image backup](./Kenwood_TK-862G_20251027-default.img) - ([commit fe3269fae9](https://gitea.rcs1.top/sickprodigy/chirp-radio/commit/fe3269fae9049abb2c514a51a72a8c148747b414))
- Frequency range: 450MHz-490MHz (Business version)
- Originally purchased for TARPN (incorrect model)
- Limitations:
  - FM reception only (no DMR/Digital)
  - Cannot access lower range of 70cm band (420MHz-449MHz)
  - May attempt frequency modification via soldering

### Kenwood TK-862G-1 (Reprogrammed)
- [Kenwood TK-862G Programmed Image](./Kenwood_TK-862G_20251027-programmed.img) - ([commit af7c92f265](https://gitea.rcs1.top/sickprodigy/chirp-radio/commit/af7c92f26537bb019bf844214ed5d6acb920b5cd))
- Contains custom frequency programming for 8 channels
- Includes local Wake County frequencies
- Backup made after successful programming session and signal was received. 

### Baofeng UV-5R (Default)
- [Baofeng UV-5R](./Baofeng_5RM_default.img) - ([commit 1318d62413](https://gitea.rcs1.top/sickprodigy/chirp-radio/commit/1318d624137ea19db09723f2d588cc75eb36b180))
- Dual-band handheld (VHF/UHF)
- DMR capable (if using compatible model)
- Used for portable operations and testing

### Baofeng UV-5R (Reprogrammed)
- [Baofeng UV-5R](./Baofeng_5RM_edited.img) - ([commit 1318d62413](https://gitea.rcs1.top/sickprodigy/chirp-radio/commit/1318d624137ea19db09723f2d588cc75eb36b180))
- Contains custom frequency programming for 8 channels
- Includes local Wake County frequencies
- Backup made after successful programming session and signal was received. 

### Future Equipment
- Planning to order TK-76x for VHF purposes
- Looking into cheaper handhelds with DMR capability
- Considering additional models for expanded frequency coverage

## RadioReference Database Usage

### Query Results Examples
- [CSV Format: Query Results - CHIRP - RadioReference.com - Wake, NC, USA](QueryResult-radioreference.com-chirp-example-NC-Wake-County.csv)
- [Excel Format: Query Results - CHIRP - RadioReference.com - Wake, NC, USA](QueryResult-radioreference.com-chirp-example-NC-Wake-County.xlsx)

### Understanding the Data
Reference Data: [RadioReference.com: Wake County Radio Systems](https://www.radioreference.com/db/browse/ctid/1978#cid-4811)

#### Example Translation
RadioReference.com Format:
```
461.9875 | WQOL325 | RM | 100.0 PL | DH Hill Library | DH Hill Library | FMN | Schools
```

CHIRP Query Result Format:
```
61 | DH Hill Library | 461.9875 | split | 466.9875 | TSQL | 100 | 100 | 023 | NN | 023 | Tone->Tone | NFM | 5 | 50W | DH Hill Library
```

### CHIRP Terminology Notes
- Standard "100.0 PL" translates to "TSQL 100.0" in CHIRP
- Planning to include more default images and examples to clarify CHIRP's unique terminology

## Contact
Sick Prodigy / Aaron

---
*Note: This repository aims to provide comprehensive information about radio programming through git version control.*