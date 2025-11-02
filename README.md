# CHIRP Radio Programming Documentation




## Introduction
This repository serves as a backup of my progress with CHIRP and radio programming experiences.

## Resources Used
I paid for access to [RadioReference.com](https://www.radioreference.com/) ($15.00) to query their database. While I only queried local results initially, I plan to expand this. Note: Many sites require monthly subscriptions for information that arguably should be freely available or donation-based, considering the already significant cost of equipment.

## Equipment

### Kenwood TK-862G-1  (Default)
- [Default image backup](./Kenwood_TK-862G_20251027-default.img)
- Frequency range: 450MHz-490MHz (Business version)
- Originally purchased for TARPN (incorrect model)
- Limitations:
  - FM reception only (no DMR/Digital)
  - Cannot access lower range of 70cm band (420MHz-449MHz)
  - May attempt frequency modification via soldering

### Kenwood TK-862G-1 (reprogrammed)
- [Kenwood TK-862G Programmed Image](./Kenwood_TK-862G_20251027-programmed.img) ([commit af7c92f265](https://gitea.rcs1.top/sickprodigy/chirp-radio/commit/af7c92f26537bb019bf844214ed5d6acb920b5cd))
- Contains custom frequency programming for 8 channels
- Includes local Wake County frequencies
- Backup made after successful programming session and signal was received. 

### Future Equipment
- Planning to order TK-76x for VHF purposes
- Looking into cheaper handhelds with DMR capability

## RadioReference Database Usage

### Query Results Examples
- [CSV Format](QueryResult-radioreference.com-chirp-example-NC-Wake-County.csv)
- [Excel Format](QueryResult-radioreference.com-chirp-example-NC-Wake-County.xlsx)

### Understanding the Data
Reference: [Wake County Radio Systems](https://www.radioreference.com/db/browse/ctid/1978#cid-4811)

#### Example Translation
RadioReference Format:
```
461.9875 | WQOL325 | RM | 100.0 PL | DH Hill Library | DH Hill Library | FMN | Schools
```

Query Result Format:
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