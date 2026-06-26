---
title: '{{ replace .File.ContentBaseName "-" " " | title }}'
date: {{ .Date }}
slug: "{{ replace .File.ContentBaseName "-" " " | title }}"
description: "default description"
author: jqx
categories: ["categorie"]
Keywords: ["key1","key2"]
tags: ["tag1","tag2"]
images:
- /banner1.png
- /banner2.png
draft: true
---
