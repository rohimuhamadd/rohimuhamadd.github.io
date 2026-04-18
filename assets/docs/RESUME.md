# MUHAMAD NUR ROHIM  
**Software Engineer (Odoo Developer with DevOps Engineer)**  
Bandung, Indonesia · HP: 081283399030 · Email: rohimuhamadd@gmail.com  
LinkedIn: rohimuhamadd · GitHub: rohimoz28 · Blog: rohimoz28.netlify

---

## RINGKASAN
Software Engineer dengan **4+ tahun** pengalaman membangun dan mengoperasikan aplikasi ERP/HR berbasis **Odoo (v16/v17)** dengan kemampuan DevOps (CI/CD, Docker, Linux, observability). Mengelola platform HR untuk **2 project** (pabrik farmasi & rumah sakit) dengan delivery multi-environment pada **7 VM Ubuntu**. Berpengalaman mengerjakan workload HR skala besar pada pabrik: **generate absensi & payroll untuk ~11.000 employee** (perkiraan) pada **12 branch (multi-company)** menggunakan optimasi **PostgreSQL query + implementasi Python**. Untuk rumah sakit saat ini dalam tahap development dengan **~6.000 employee** (perkiraan).

---

## HIGHLIGHTS (IMPACT)
- Mengelola ekosistem **7 VM Ubuntu**: 2 production (pisah project&server), 2 staging (pisah), 1 dev platform (GitLab + Runner + technical blog), Metabase, n8n.  
- Menjalankan delivery harian dengan **auto-deploy on merge** dan rata-rata **8 CI/CD job/hari**; waktu deploy **±3 menit/job** (start → notifikasi Discord).  
- Backup/restore database terpusat melalui **GitLab Scheduled pipelines** + manual trigger: total data **hingga 120GB** (maks **~100GB** per DB), output **split + gzip (.gz)**.  
- Reliability target **99.9%**; recovery release via **rollback commit** bila issue, lalu perbaikan dari branch hasil checkout kondisi error.  
- Mengadaptasi **GitLab Flow** untuk tim dengan banyak junior: standar branching/merge/release yang menurunkan risiko human error.

---

## SKILL TEKNIS
**Odoo & Backend (Core):** Odoo v16/v17, ORM, QWeb PDF, Custom Modules, Reporting, Access/Record Rules, Multi-company, Workflow Automation  
**Database (Core):** PostgreSQL (query tuning, indexing, batch processing skala besar)  
**DevOps & Infra (Core):** Docker Compose, Nginx (reverse proxy / request forwarding), GitLab CI/CD, GitLab Runner, Bash, Linux (Ubuntu VM; familiar Fedora/Debian)  
**Observability (Core):** Grafana, Loki  
**Programming (Core):** Python  
**Additional:** PHP, Laravel, CodeIgniter

---

## PENGALAMAN KERJA

### PT SANBE FARMA — Bandung, Indonesia  
**Lead Dev & DevOps** (Aug 2024 – Sekarang)

**Delivery & Release Engineering**
- Mendesain alur release: **local testing di laptop developer** (port forwarding via **Nginx + cloudflared**) → deploy **staging** → deploy **production**.  
- Mengimplementasikan pipeline deployment **auto on merge** (tanpa approval gate; review & deploy oleh lead), dengan standar recovery: **rollback commit** bila issue lalu perbaikan dari branch hasil checkout kondisi error.  
- Menjalankan rata-rata **8 CI/CD job/hari** dengan durasi deploy **±3 menit/job**, notifikasi **per job** ke Discord.

**Platform & Infrastructure**
- Mengelola arsitektur multi environment pada **7 VM Ubuntu**:
  - 2 production (pabrik & rumah sakit), 2 staging (pabrik & rumah sakit),
  - 1 dev platform (GitLab, GitLab Runner, technical blog),
  - 1 Metabase, 1 n8n.  
- Mengoperasikan Odoo di **Docker Compose** dengan **PostgreSQL container** (satu stack), serta Nginx untuk **forward request antar server**.

**Odoo Engineering (HR Skala Besar)**
- Pabrik farmasi: membangun proses HR skala besar untuk **~11.000 employee** (perkiraan) pada **12 branch (multi-company)**:
  - Menyusun **query PostgreSQL** untuk **generate absensi** skala besar, lalu mengintegrasikannya ke Odoo melalui implementasi **Python**.  
  - Payroll (ongoing): mengembangkan proses **allowance & deduction** berbasis absensi dan komponen payroll menggunakan query PostgreSQL + integrasi Odoo.  
	- Rumah sakit (development): menyiapkan modul HR untuk **~6.000 employee** (perkiraan).

**Observability & Monitoring**
- Membangun dashboard Grafana untuk:
  - **monitoring resource server**,  
  - **log Odoo** (via Loki),  
  - **realtime stage tracking** untuk Project Management menggunakan **query PostgreSQL**.  

**Ops Automation (Backup/Restore)**
- Mengorkestrasi backup & restore database via **GitLab Scheduled pipelines** dan manual trigger:
  - total data hingga **120GB** (maks ~100GB per DB),
  - output **split + gzip (.gz)**,
  - notifikasi Discord **per job**.

> Engineering proof (blog):  
> - Backup orchestrator: rohimoz28.netlify.app/blog/technical-blog-backup-orchestrator/  
> - PostgreSQL async replication concept: rohimoz28.netlify.app/blog/postgresql-async-replication-concept/

---

### PT DATA SISTEM SOLUSINDO — Jakarta, Indonesia  
**Web Developer** (Oct 2022 – Jul 2024)
- Mengembangkan dan memelihara sistem HRIS menggunakan **PHP (CodeIgniter)** serta website untuk kebutuhan client.  
- Melakukan customization Odoo module/report untuk mendukung proses ERP.  
- Mengembangkan aplikasi logistik dan quality control, serta maintenance aplikasi Salesforce.

### SAE MANDIRI INFORMATICS — Tangerang, Indonesia  
**Web Developer (Intern)** (Feb 2022 – Aug 2022)
- Mengembangkan aplikasi POS berbasis web dari konsep hingga deployment, termasuk training client.

---

## SELECTED PROJECT HIGHLIGHTS
- **Attendance Generator (multi-company, ~11K employee):** desain query PostgreSQL untuk generate absensi skala besar + integrasi Python di Odoo.  
- **Project Workflow + Delivery Visibility:** stage change otomatis kirim notif Discord + link, plus realtime tracking di Grafana via query PostgreSQL.  
- **Payroll Allowance/Deduction (ongoing):** perhitungan allowance/deduction berbasis absensi & komponen payroll untuk skala besar.  
- **Backup Orchestrator (GitLab Scheduled):** backup/restore terpusat, split + gzip, notifikasi Discord per job.

---

## PORTFOLIO
- Setup Odoo Dev: https://github.com/rohimoz28/setup-odoo-dev  
- Learn Odoo Basic: https://github.com/rohimoz28/learn-odoo-basic  
- PostgreSQL Async Replication Lab: https://github.com/rohimoz28/lab-postgresql-async-replication  
- Blog Source: https://github.com/rohimoz28/rohimoz28-blog

---

## PENDIDIKAN
**Bina Sarana Informatika** (2013 – 2016) — D3 Manajemen Informatika · IPK 3.05

---

## SERTIFIKASI (KURASI)
- Odoo Technical Training (Arkana, 2024)  
- Docker, PostgreSQL, Laravel/PHP (Programmer Zaman Now / Udemy)