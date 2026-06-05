# move-tech-cloud-application-comp-3

Ponto de partida da **Competência 3 — Desenvolvimento e Operação de Aplicações (DevOps)**.

Este repositório é um template. Use-o como base para criar o seu próprio repositório e trabalhar na competência.

> Parte do curso **Move Tech** — Magalu × Prósper Digital Skills  
> Formação em Cloud Computing para iniciantes

---

## O que tem aqui

Uma API simples de micro e-commerce com pedidos e itens, construída em Python com FastAPI.

A aplicação armazena os dados em memória. Ainda não tem deploy na nuvem — isso é exatamente o que você vai fazer nesta competência.

### Endpoints disponíveis

| Método | Rota | Descrição |
|--------|------|-----------|
| `GET` | `/health` | Verifica se a API está no ar |
| `POST` | `/orders` | Cria um novo pedido |
| `GET` | `/orders` | Lista todos os pedidos |
| `GET` | `/orders/{id}` | Retorna um pedido com seus itens |
| `DELETE` | `/orders/{id}` | Cancela um pedido |
| `POST` | `/orders/{id}/items` | Adiciona um item ao pedido |
| `GET` | `/orders/{id}/items` | Lista os itens de um pedido |

---

## O que você vai fazer nesta competência

Ao final da Competência 3, a aplicação deve estar **versionada, conteinerizada e publicada na Magalu Cloud**.

- [ ] Publicar a imagem no Container Registry da Magalu Cloud
- [ ] Criar os manifests Kubernetes (`k8s/deployment.yaml` e `k8s/service.yaml`)
- [ ] Fazer o deploy no cluster Kubernetes da Magalu Cloud
- [ ] Configurar o pipeline de CI/CD no GitHub Actions

---

## Como rodar localmente

**Pré-requisito:** [Docker Desktop](https://www.docker.com/products/docker-desktop/) instalado (Mac e Windows) ou [Docker Engine](https://docs.docker.com/engine/install/) (Linux).

```bash
docker compose up --build
```

Acesse a documentação interativa em: http://localhost:8000/docs

---

## Próxima etapa

Ao concluir esta competência, a solução de referência será publicada em:  
[move-tech-cloud-application-comp-4](https://github.com/move-tech-cloud-computing/move-tech-cloud-application-comp-4)

---

> Inspirado no tutorial [Construindo APIs robustas utilizando Python](https://github.com/luizalabs/tutorial-python-brasil) do LuizaLabs.
