# Homelab

Bem-vindo à organização **davidcardoso-homelab**!  
Aqui você encontra um conjunto de repositórios para provisionar, monitorar e gerenciar um ambiente Kubernetes completo para homelab, utilizando práticas modernas de infraestrutura como código e GitOps.

## Visão Geral

Este projeto foi desenvolvido para facilitar a criação de um ambiente de laboratório doméstico (homelab) robusto, modular e facilmente reprodutível.  
A stack contempla desde a instalação do cluster Kubernetes até a configuração de serviços de mídia, DNS seguro, monitoramento e balanceamento de carga.

---

## Ordem Recomendada de Instalação

Para reproduzir o ambiente completo, siga a ordem abaixo:

1. [**k3s**](https://github.com/davidcardoso-homelab/k3s)  
	Provisionamento automatizado do cluster Kubernetes (k3s), scripts de instalação e configuração inicial.

2. [**monitoring**](https://github.com/davidcardoso-homelab/monitoring)  
	Stack de monitoramento baseada em kube-prometheus-stack (Prometheus, Grafana, Alertmanager), totalmente gerenciada via ArgoCD.

3. [**metallb**](https://github.com/davidcardoso-homelab/metallb)  
	Balanceador de carga de IPs para Kubernetes em ambientes bare-metal, permitindo exposição de serviços via LoadBalancer.

4. [**pihole-unbound**](https://github.com/davidcardoso-homelab/pihole-unbound)  
	Solução de DNS seguro e privado, combinando Pi-hole (bloqueio de anúncios) e Unbound (resolução recursiva).

5. [**media**](https://github.com/davidcardoso-homelab/media)  
	Central de mídia com Jellyfin, Sonarr, Radarr, qBittorrent, Bazarr, Prowlarr, Homarr e Jellyseerr, todos orquestrados via Kubernetes.

6. [[**kubernetes-dashboard**]](https://github.com/davidcardoso-homelab/kubernetes-dashboard)  
	Solução web para visualizar o cluster através de uma interface amigável.

---

## Como Utilizar

Cada repositório possui um README detalhado com instruções de instalação, pré-requisitos e exemplos de configuração.  
Siga rigorosamente a ordem acima para garantir que todas as dependências estejam corretamente configuradas.

- **Pré-requisitos gerais:**  
  - Linux com permissões de sudo  
  - Git instalado  
  - Familiaridade básica com Kubernetes e kubectl

- **GitOps:**  
  Todos os componentes são gerenciados via [ArgoCD](https://argo-cd.readthedocs.io/), permitindo versionamento, automação e fácil replicação do ambiente.

---

## Suporte e Contribuição

- Dúvidas, sugestões ou problemas? Abra uma issue no repositório correspondente.
- Contribuições são bem-vindas! Consulte as diretrizes de contribuição em cada projeto.

---

> Desenvolvido e mantido por [David Rafael Cardoso](https://github.com/davidcardoso01)
