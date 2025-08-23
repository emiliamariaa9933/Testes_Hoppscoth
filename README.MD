# 🧪 Testes Hoppscotch - Execução Local e CI via GitHub Actions

Este repositório contém collections e variáveis de ambiente para executar testes de API com o Hoppscotch CLI, gerar relatórios JUnit e integrar com GitHub Actions.

---

## 🚀 Executando os testes localmente

### 1. Instale o Hoppscotch CLI e o JUnit Viewer globalmente:

```bash
npm install -g @hoppscotch/cli junit-viewer
```


### 2. Execute a collection com os testes, passando o arquivo de variaveis de ambiente:

```bash
hopp test -e scripts-hoppscotch/environments/Global.json -d 1000 scripts-hoppscotch/collections/testes_api.json --reporter-junit results/report.xml
```

### 3. Gerar relatório HTML a partir do XML

```bash
junit-viewer --results=results/report.xml --save=results/report.html
```

