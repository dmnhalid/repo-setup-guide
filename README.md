<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:16213e&height=180&section=header&text=repo-setup-guide&fontSize=44&fontColor=7CFFB2&fontAlignY=38&desc=Profesyonel%20bir%20repo%20nas%C4%B1l%20kurulur%3F%20%E2%80%94%20Ad%C4%B1m%20ad%C4%B1m%20rehber&descAlignY=58&descSize=14&descColor=8892b0&animation=fadeIn" />

</div>

<br/>

> Sıfırdan profesyonel bir GitHub/GitLab deposu kurmak için gereken her şey: CI/CD, lisans, changelog, Kubernetes, observability ve daha fazlası. Her bölüm kendi klasöründe, açıklama + çalışan kod örnekleriyle.

---

## Konular

| # | Konu | Açıklama | Durum |
|---|------|----------|-------|
| 01 | [README](./01-readme) | Etkili README nasıl yazılır, şablonlar | ⬜ |
| 02 | [CI/CD Configuration](./02-cicd) | GitHub Actions & GitLab CI pipeline kurulumu | ⬜ |
| 03 | [LICENSE](./03-license) | Lisans türleri, nasıl seçilir, nasıl eklenir | ⬜ |
| 04 | [CHANGELOG](./04-changelog) | Keep a Changelog formatı, semantic versioning | ⬜ |
| 05 | [CONTRIBUTING](./05-contributing) | Katkı rehberi, PR şablonu, branch stratejisi | ⬜ |
| 06 | [Kubernetes](./06-kubernetes) | Deployment, Service, Ingress, ConfigMap örnekleri | ⬜ |
| 07 | [Wiki](./07-wiki) | Repo wiki yapısı, dokümantasyon standartları | ⬜ |
| 08 | [Integrations](./08-integrations) | Slack, Jira, SonarCloud, Dependabot bağlantıları | ⬜ |
| 09 | [Observability](./09-observability) | Prometheus, Grafana, alert kuralları, dashboard | ⬜ |

> ⬜ Bekliyor · 🔄 Devam ediyor · ✅ Tamamlandı

---

## Klasör yapısı

```
repo-setup-guide/
│
├── 01-readme/
│   ├── README.md          ← Açıklama
│   └── templates/         ← Hazır şablonlar
│
├── 02-cicd/
│   ├── README.md
│   ├── github-actions/    ← .github/workflows/ örnekleri
│   └── gitlab-ci/         ← .gitlab-ci.yml örnekleri
│
├── 03-license/
│   ├── README.md
│   └── examples/          ← MIT, Apache, GPL örnekleri
│
├── 04-changelog/
│   ├── README.md
│   └── CHANGELOG.md       ← Örnek changelog
│
├── 05-contributing/
│   ├── README.md
│   ├── CONTRIBUTING.md    ← Örnek katkı rehberi
│   └── pull_request_template.md
│
├── 06-kubernetes/
│   ├── README.md
│   └── manifests/         ← deployment.yaml, service.yaml vb.
│
├── 07-wiki/
│   ├── README.md
│   └── structure/         ← Wiki sayfa şablonları
│
├── 08-integrations/
│   ├── README.md
│   └── configs/           ← dependabot.yml, sonar-project.properties
│
└── 09-observability/
    ├── README.md
    └── configs/           ← prometheus.yml, grafana dashboard JSON
```

---

## Her klasörün içeriği

Her bölüm şu yapıyı takip eder:

```
XX-konu/
├── README.md     ← Ne işe yarar · Ne zaman kullanılır · Nasıl kurulur · Örnekler
└── ...           ← Konuya özgü dosyalar (yaml, json, md şablonları)
```

---

## Nasıl kullanılır?

İstediğin konuya git, README'yi oku, dosyaları kendi projena kopyala ve gerekli yerleri düzenle.

```bash
# Örnek: CI/CD dosyalarını kendi projena almak
cp -r 02-cicd/github-actions/.github /your-project/
```

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16213e,50:1a1a2e,100:0d1117&height=100&section=footer&animation=fadeIn" />
<sub><code>// built step by step — dmnhalid</code></sub>
</div>
