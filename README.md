<p align="center">
  <img alt="Profile README" src="https://img.shields.io/badge/Profile-README-2E86AB?style=for-the-badge">
  <img alt="Idioma" src="https://img.shields.io/badge/Idioma-PT--BR-27AE60?style=for-the-badge">
</p>

<p align="center">
  <img alt="GIWNLTREMA" src="https://img.shields.io/badge/GIWNLTREMA-DBRE%20%7C%20DBA%20%7C%20Cloud-2ECC71?style=for-the-badge&labelColor=1B2631">
</p>

<p align="center">
  <img alt="DBRE Animated Banner" src="assets/dbre-animated-banner.svg">
</p>

<p align="center">
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-Database%20Platform-326CE5?style=flat-square&logo=kubernetes&logoColor=white">
  <img alt="Argo CD" src="https://img.shields.io/badge/Argo%20CD-GitOps-EF7B4D?style=flat-square&logo=argo&logoColor=white">
  <img alt="Crossplane" src="https://img.shields.io/badge/Crossplane-Compositions-3E5C9A?style=flat-square&logo=crossplane&logoColor=white">
  <img alt="Grafana" src="https://img.shields.io/badge/Grafana-Observabilidade-F46800?style=flat-square&logo=grafana&logoColor=white">
  <img alt="Prometheus" src="https://img.shields.io/badge/Prometheus-Metricas-E6522C?style=flat-square&logo=prometheus&logoColor=white">
  <img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-Foco%20Principal-47A248?style=flat-square&logo=mongodb&logoColor=white">
</p>

# giwnltrema

DBRE com foco em resiliencia de bancos, operacao GitOps e automacao de plataforma para reduzir toil de DBA/SRE.

## Sumario

- [O que voce encontra aqui](#o-que-voce-encontra-aqui)
- [Arquitetura de trabalho](#arquitetura-de-trabalho)
- [Agora](#agora)
- [Especialidades tecnicas](#especialidades-tecnicas)
- [Projeto em foco](#projeto-em-foco)
- [MongoDB highlights](#mongodb-highlights)
- [Metricas do perfil](#metricas-do-perfil)
- [Contato](#contato)

## O que voce encontra aqui

| Area | Entrega |
|---|---|
| DBRE | Padroes para bancos clusterizados em Kubernetes com foco em RTO/RPO e failover seguro |
| GitOps | Fluxo de provisionamento por PR com ArgoCD, policies e trilha auditavel |
| Observabilidade | Dashboards, alertas e query insights para enxergar lag, lock, custo e saude real |
| Backup/DR | Backup continuo com restore validado para evitar risco oculto |

## Arquitetura de trabalho

```mermaid
flowchart LR
    PR[Pull Request] --> ARGO[Argo CD]
    ARGO --> CP[Control Plane DBRE]
    CP --> DB[(Cluster de Banco)]
    DB --> OBS[Prometheus + Grafana + Loki]
    DB --> BKP[Backup + Restore Validation]
    OBS --> SCORE[Scorecard de Confiabilidade]
    BKP --> SCORE
```

## Agora

- Construindo um control plane DBRE para Kubernetes com composicoes, policies e onboarding rapido.
- Padronizando backup por engine com restore de validacao e telemetria de sucesso.
- Estruturando um caminho de produto no modelo open-core + camada SaaS.

## Especialidades tecnicas

| Pilar | Stack principal |
|---|---|
| Bancos | MongoDB, Postgres, MySQL |
| Kubernetes DB | Patroni, PXC/ProxySQL, operadores de banco |
| Cloud/Infra | AWS, Kubernetes, Terraform, Helm, Crossplane |
| GitOps | ArgoCD, repos declarativos, pipelines de reconciliacao |
| Observabilidade | Prometheus, Grafana, Loki, Alertmanager |
| Automacao | Python, PowerShell, Bash, GitHub Actions |

## Projeto em foco

- [`dbre-control-plane`](https://github.com/giwnltrema/dbre-control-plane): visao de plataforma para bancos clusterizados com GitOps, observabilidade integrada e backup validado.
- [`terrariadosbobo`](https://github.com/giwnltrema/terrariadosbobo): referencia visual e pratica de stack orientada a operacao, metricas e GitOps.

## MongoDB highlights

- Operacao de replica set e shard com foco em estabilidade e padrao operacional.
- Backup/restore com verificacao periodica e monitoramento de freshness.
- Tuning de performance com indices, profiler e analise de workload.
- Planejamento de resiliencia com game days e validacao de failover.

## Metricas do perfil

<p>
  <img src="https://github-readme-stats.vercel.app/api?username=giwnltrema&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com?user=giwnltrema&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>
<p>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=giwnltrema&layout=compact&theme=tokyonight&hide_border=true&langs_count=6&hide=shell" alt="Top Langs" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=giwnltrema&label=visitas&color=4F46E5&style=flat-square" alt="Visitantes">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/giwnltrema/giwnltrema/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/giwnltrema/giwnltrema/output/github-snake.svg" />
    <img alt="github-snake" src="https://raw.githubusercontent.com/giwnltrema/giwnltrema/output/github-snake.svg" />
  </picture>
</p>

## Contato

<p align="left">
  <a href="https://www.linkedin.com/in/gabrielfdbre/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://discord.gg/trema"><img src="https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white" alt="Discord"></a>
  <a href="https://github.com/giwnltrema"><img src="https://img.shields.io/badge/GitHub-0f172a?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
</p>
