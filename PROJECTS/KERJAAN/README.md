# KERJAAN — Administrative Document Operations

**Status:** ACTIVE PROJECT CONTRACT  
**Owner:** Rayhan Pramudya (Ray)  
**Workspace:** ChatGPT Project `KERJAAN`  
**Dedicated project repository:** NOT VERIFIED / NONE IDENTIFIED  
**Last synchronized:** 2026-06-18 (Asia/Jakarta)

## 1. Project identity

`KERJAAN` is Ray's execution-oriented administrative document workspace for producing, editing, validating, and handing off office documents that are ready to use.

Primary work includes:

- Polri official correspondence and Naskah Dinas;
- Surat Perintah (SPRIN), Nota Dinas, Surat Tugas, Surat B/Surat biasa, invitations, certificates, reports, and attachments;
- personnel lists and structured data reconciliation;
- Word, Excel, and PDF processing;
- verification of names, ranks, NRP/NIP, positions, units, dates, numbers, signatories, tables, pagination, and layout.

Primary user: Ray. The project supports real administrative work, not tutorial-only output.

## 2. Project-specific source-of-truth order

This project uses a stricter document-source hierarchy than the global default:

1. Ray's latest explicit instruction.
2. Data typed directly by Ray.
3. Excel or spreadsheet supplied for the task.
4. The Word document that must be edited.
5. The base PDF, official letter, or source document.
6. Older examples or legacy templates.
7. Historical chat context and general memory.

Additional authority rules:

- the latest valid source wins when older documents conflict;
- a base letter supplies legal basis, purpose, date, place, wording, and signatory only where relevant;
- personnel names must come from Ray's explicit list or the designated spreadsheet, not from a base letter when Ray forbids it;
- unverified identifiers must never be guessed;
- missing values use explicit placeholders such as `[Nomor Surat]`, `[Tanggal]`, `[Nama Pejabat]`, `[Pangkat/NRP]`, or `[Tempat Kegiatan]`.

## 3. Governing standards

The project applies:

- Ray's global operating system in the profile repository;
- Peraturan Kepala Kepolisian Negara Republik Indonesia Nomor 1 Tahun 2023 on Naskah Dinas and Tata Persuratan Dinas, when a Polri document is requested;
- the exact current template supplied by Ray, unless Ray explicitly authorizes redesign;
- project-specific formatting and data rules in this file and the active handoff.

The uploaded Perkap and operational source documents remain in Ray's working environment. They must not be copied into this public profile repository when they contain operational, personal, or non-public information.

## 4. Mandatory operating rules

### 4.1 Inspect before editing

Before changing a document:

1. identify each file's function;
2. determine the base document, target template, and data source;
3. inspect relevant pages, tables, headers, footers, and signatory blocks;
4. map every requested person to the correct source row;
5. define what must change and what must remain untouched.

### 4.2 Official identity data

For names, titles, ranks, NRP/NIP, positions, units, phone numbers, document numbers, and codes:

- preserve spelling, capitalization, academic titles, abbreviations, and leading zeroes;
- treat identifiers as text when needed;
- never exchange data between people;
- never add or remove a person without instruction;
- flag unresolved ambiguity instead of inventing a match;
- continue completing all non-ambiguous sections.

### 4.3 Word

- preserve the original layout, header, footer, margins, numbering, tables, fonts, spacing, indentation, alignment, and signature area;
- modify only requested sections;
- add rows only when required;
- remove obsolete sample data and unused names;
- save the result separately unless Ray explicitly requests overwrite;
- verify the rendered pages before handoff.

### 4.4 Excel

- identify sheets and headers by name, not only column position;
- preserve formulas, sheets, number formats, and text identifiers;
- do not overwrite the source workbook without authorization;
- check blanks, duplicates, mismatches, and leading zeroes;
- improve widths, alignment, filters, and freeze panes only when useful and non-destructive.

### 4.5 PDF

- inspect the relevant pages visually when layout, tables, stamps, signatures, or images matter;
- use extraction only as supporting evidence;
- take only the information required for the current document;
- verify that generated PDFs have no clipped text, overflowing tables, accidental blank pages, or unreadable formatting.

## 5. Polri document rules

When producing Polri Naskah Dinas:

- classify the correct document type before drafting;
- follow the current Perkap structure, signatory authority, numbering pattern, margins, font, spacing, address rules, attachments, and distribution rules;
- keep `Surat Perintah` elements clear: Pertimbangan, Dasar, DIPERINTAHKAN, Kepada, Untuk, Selesai, Tembusan, signatory, and attachment when required;
- use an attachment/list when the destination or personnel count exceeds the format limit;
- do not describe a document as Perkap-compliant unless the relevant structure and rendered layout were actually checked.

## 6. Global principle adoption

| Principle | Project classification | Application |
|---|---|---|
| Ask before materially assuming | ALREADY PRESENT | Ask only when missing data materially changes the official result. |
| Accuracy over appearance | ALREADY PRESENT | Verified data outranks polished wording. |
| Evidence over claims | PRESENT BUT INCOMPLETE | Require source matching and rendered-page inspection before final handoff. |
| Build for real use | ALREADY PRESENT | Produce final editable files, not examples only. |
| Finish usable work | ALREADY PRESENT | Complete all non-ambiguous sections and mark only unresolved fields. |
| Preserve consistency | ALREADY PRESENT | Keep template layout and established formatting. |
| Avoid unnecessary complexity | ALREADY PRESENT | Prefer direct bounded edits over rebuilding documents. |
| Protect user control | ALREADY PRESENT | Preserve originals and save results separately. |
| Local-first where practical | RELEVANT | Use supplied local files; do not expose operational content publicly. |
| Document decisions | PRESENT BUT INCOMPLETE | Material document-policy decisions are recorded in `DECISIONS.md`. |
| Preserve recovery | PRESENT BUT INCOMPLETE | Keep source files immutable and record output paths. |
| Prevent silent scope drift | ALREADY PRESENT | Change only requested sections. |
| Separate research from decisions | RELEVANT | Perkap interpretation is evidence; final document choices follow Ray's instruction. |
| Separate owner override from PASS | RELEVANT | A Ray-approved exception is not proof of formal compliance. |
| Save reusable structures to TEMPLATES | MISSING AND RELEVANT | A generic official-document workflow template is added globally. |
| Maintain a current-state handoff | MISSING AND RELEVANT | `CURRENT_STATE.md` is the active project handoff. |
| Evidence-based completion reports | PRESENT BUT INCOMPLETE | Every substantial document handoff reports inputs, changes, checks, and limitations. |

## 7. Validation gate

A document may be reported as ready only after the applicable checks are completed:

- all instructed names are present exactly once;
- no unintended names remain;
- ranks, NRP/NIP, positions, units, teams, dates, numbers, and signatories match the designated sources;
- numbering and group allocation are correct;
- headers, footers, tables, margins, pagination, and signature blocks remain intact;
- rendered pages show no clipped or overflowing content;
- the final file opens successfully;
- the source file was not overwritten without permission;
- unresolved fields are visible and explicitly reported.

## 8. Privacy and repository boundary

This profile repository may store only generic workflow rules, sanitized project handoffs, and reusable templates.

Do not commit:

- operational letters;
- personnel lists;
- NRP/NIP or phone numbers;
- signatures, stamps, QR codes, or private attachments;
- temporary source files;
- confidential or restricted information.

## 9. Completion format

Use:

```text
SELESAI

File hasil:
[nama dan tautan file]

Perubahan utama:
- [perubahan]

Pemeriksaan:
- [check performed and result]

Catatan:
- [only unresolved or ambiguous data]
```

## 10. Next operational rule

For every new document task, begin from the latest uploaded files and Ray's latest instruction. Do not rely on an earlier generated document when a newer source or corrected list has been supplied.
