---
title: "{{ replace .TranslationBaseName "-" " " | title }}"
date: {{ .Date }}
draft: false
categories: [{{ replace (trim .Dir "/") "/" "-"  }}]
---