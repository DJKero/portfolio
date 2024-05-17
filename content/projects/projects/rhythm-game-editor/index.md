---
title: Rhythm Game Editor
date: 2024-05-07T03:00:00.000Z
categories:
    - Project
lastmod: 2024-05-07T03:00:00.000Z
preview: feature*BmsONE.png
showTableOfContents: true
---

{{< lead >}}
I'm currently maintaining a fork of an open source rhythm game content editor called BmsONE.  
It is an editor for the open format specification [BMSON](https://bmson-spec-fork.readthedocs.io/en/latest/doc/index.html#general), which I also forked and been working on.  
{{< /lead >}}

## Description

The [BMSON](https://bmson-spec-fork.readthedocs.io/en/latest/doc/index.html#general) format is the successor to the [BMS](https://en.wikipedia.org/wiki/Be-Music_Source) format.  
The key feature of these formats are the **Keysounds**, pioneered by KONAMI's [Beatmania](https://en.wikipedia.org/wiki/Beatmania), the user's actions trigger sounds corresponding to the notes played. These were decided at the time of production and exported separately from the song's **BGM** (Background Music).  
The previous format had a limit on the maximum number of **Keysounds** available to use.

The [BMSON](https://bmson-spec-fork.readthedocs.io/en/latest/doc/index.html#general) format eliminates this technical limitation while also providing a better production environment for the content creators.  
The song producer can export each **SFX** and **Instrument Track** separately.  
The song can be arranged in the editor by the song producer or the level creator once and be saved as a template for level creation.  

The format is way more flexible for content creation because the responsibility for cutting the sounds is delegated to the game itself, meaning that every single **SFX** or part of an **Instrument Track** can be used as a note.  

The editor is built with Qt and written in C++.  
There's a lot of work to do in this project ranging from fixing deprecation and compiler warnings, fixing memory issues like memory leaks, fixing crashes, and adding functionality to improve the user's workflow, compared to existing [BMS](https://en.wikipedia.org/wiki/Be-Music_Source) editors.  

## Screenshots  

{{< figure src="feature*BmsONE.png" alt="Editor screenshot">}}  

## Repositories

### Main repository  
{{< github repo="djkero/BmsONE" >}}  

### Format specification repository  
{{< github repo="djkero/bmson-spec-fork" >}}  