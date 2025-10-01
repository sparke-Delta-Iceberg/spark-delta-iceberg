---
title: Troubleshooting
---

## Problemas comuns

### Erro: materialx.emoji não encontrado
Atualize o `mkdocs.yml` para usar `material.extensions.emoji`.

```yaml
pymdownx.emoji:
  emoji_index: !!python/name:material.extensions.emoji.twemoji
  emoji_generator: !!python/name:material.extensions.emoji.to_svg
```

### PySpark não encontra Java
Instale o OpenJDK 17 e defina `JAVA_HOME` (ver `setup/environment.md`).

### Kernel errado no Jupyter
Selecione o kernel `.venv` ao abrir o notebook.


