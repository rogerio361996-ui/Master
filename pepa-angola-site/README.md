# PEPA — Plataforma de Economia Petrolífera Angolana

Relatório analítico autónomo sobre a economia petrolífera angolana (2000–2033),
com Machine Learning (Regressão Linear + Random Forest) e a Conjectura de Collatz.

Todo o site está contido num único ficheiro `index.html` — não é necessário
instalar nada nem executar qualquer passo de build.

## Conteúdo da pasta

| Ficheiro     | Descrição                                                    |
|--------------|--------------------------------------------------------------|
| `index.html` | O site completo (HTML + CSS + JavaScript no mesmo ficheiro)  |
| `README.md`  | Este documento                                                |
| `LICENSE`    | Licença MIT                                                   |
| `.nojekyll`  | Impede o processamento Jekyll no GitHub Pages                 |
| `.gitignore` | Ficheiros de sistema a ignorar no Git                         |

## Publicar no GitHub Pages (5 minutos)

1. Crie um repositório novo em https://github.com/new (pode ser público).
2. Envie **o conteúdo desta pasta** para a raiz do repositório:
   `Add file` → `Upload files` → arraste tudo → `Commit changes`.
3. No repositório, abra `Settings` → `Pages`.
4. Em *Source*, escolha `Deploy from a branch`.
5. Em *Branch*, escolha `main` e a pasta `/ (root)` → `Save`.
6. Aguarde 1–2 minutos. O site fica disponível em:
   https://SEU-UTILIZADOR.github.io/NOME-DO-REPOSITORIO/

### Alternativa por linha de comandos

```
git init
git add .
git commit -m "PEPA - relatorio ML"
git branch -M main
git remote add origin https://github.com/SEU-UTILIZADOR/NOME-DO-REPOSITORIO.git
git push -u origin main
```

Depois active o GitHub Pages como nos passos 3–6.

## Funcionalidades do site

- Previsão IEPA/OSEGI para 2027–2033 (Regressão Linear, Random Forest e Ensemble)
- Cinco cenários da Conjectura de Collatz: n = 3, 10, 21, 64 e 128
- Política governamental: Péssima (-12%), Moderada (0%) e Óptima (+8%)
- Dados históricos de Angola de 2000 a 2025
- Importância das variáveis, métricas R² / RMSE / MAE e gráficos interativos
- Interface bilingue (Português / English)

## Notas técnicas

- Nenhum build é necessário: o ficheiro é 100% autónomo.
- O único recurso externo é a biblioteca Chart.js, carregada por CDN — é
  necessária ligação à internet para ver os gráficos.
- Para funcionar 100% offline, descarregue `chart.umd.min.js` para uma pasta
  `assets/` e substitua o URL do CDN dentro do `index.html`.

## Autor

Rogério Bernardo Manuel — 2026
