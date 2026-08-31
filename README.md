<p align="center">
  <img src="https://sncfoundation.github.io/logos/sheetgres.svg" width="96" alt="Sheetgres logo">
</p>

<h1 align="center">Sheetgres</h1>

<p align="center"><b>A relational database whose tables are tabs — and it already speaks SQL.</b><br>
A <a href="https://sncfoundation.github.io">Sheet-Native Computing Foundation</a> project · the spreadsheet-native <b>PostgreSQL</b></p>

---

**Status:** 📝 Unsaved Draft (design). Data & Storage TAG.

## The mapping

- **table** = a tab, **row** = a row, **column** = a column.
- **SELECT/WHERE/GROUP BY/ORDER BY/LIMIT** via the built-in `QUERY()` function (Google Visualization Query Language) — SQL out of the box.
- **PK/FK/constraints** = data validation + Apps Script triggers; **JSON** columns = JSON-in-cell.

## Honest limit

No real **transactions/ACID** (LockService is coarse, no rollback); **JOINs** are weak (QUERY doesn't join — use Apps Script/VLOOKUP).

## Connect with real clients

Paired with [SheetWire](https://github.com/sncfoundation/sheetwire), real PostgreSQL clients can connect to a Google Sheet over the native wire protocol.

- 🗺️ [SNCF Landscape](https://sncfoundation.github.io/landscape.html) · 🧩 [Projects](https://sncfoundation.github.io/projects.html) · 🎓 [Certification](https://sncfoundation.github.io/certification.html)

---

<sub>Apache-2.0. Do not run production data on a spreadsheet. If you do, please film the query plan.</sub>
