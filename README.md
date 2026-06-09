# DevOps Bootcamp 2026 — Portfolio

Repo peribadi untuk semua kerja amali bootcamp. **Satu repo, tumbuh setiap sesi.**

`main` simpan README + `.gitignore` sahaja. Setiap topik masuk melalui **cabang + PR**.

## Ritual setiap sesi

```bash
git checkout -b <sesi>            # cth: aws1, docker1, terraform1
mkdir <sesi>                      # folder artefak sesi
# ... tambah artefak SELAMAT: output, nota, Dockerfile, .tf, .github/workflows ...
git add .
git commit -m "<Sesi>: <ringkasan>"
git push -u origin <sesi>
gh pr create --fill
gh pr merge --squash --delete-branch
```

Hantar **pautan PR** ke LMS = bukti siap.

## Keselamatan

JANGAN commit kredential. `.gitignore` halang `*.csv`, `credentials`, `.aws/`, `*.pem`, `*.env`.
Access key / secret / kata laluan tidak pernah masuk repo.
