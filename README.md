# Dağıtık görev kuyruklarında worker arızaları ve görev kurtarma

**Süleyman Demirel Üniversitesi — Dağıtık Sistemler, 2026–2027 Güz**  
**Öğrenci:** Emre Kurum

Bu depo, Dağıtık Sistemler dersi vize araştırma raporunun PDF ve LaTeX kaynaklarını içerir. Çalışma, Celery/Redis üzerinde birden fazla worker ile görev devri, onay (acknowledgement), idempotency ve veritabanında tekrar kayıt oluşumu üzerine bir **deney tasarımıdır**. Vize aşamasında deney sonuçları üretilmemiştir.

## Dosyalar

- `main.pdf`: Vize ara raporu (IEEE iki sütunlu, 10 sayfa).
- `main.tex`: LaTeX metni.
- `references.bib`: Kaynakça kayıtları.
- `IEEEtran.cls`, `IEEEtran.bst`: Şablon ve bibliyografya stili.
- `figures/`: LaTeX/TikZ diyagram kaynakları.

## Yerel derleme

LaTeX, BibTeX ve gerekli TikZ paketleri kuruluysa:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

Resmî IEEEtran şablonuna dayalı olarak derlenmiştir. Bu depo, ders platformundaki asıl teslimin yerine geçmez; teslim bağlantısı ve gerekli kontroller dersin yönergesine göre yapılmalıdır.
