---
title: GPU Accelerated Machine Learning Training im Windows-Subsystem für Linux
description: Erfahren Sie mehr über die Unterstützung von WSL 2 für NVIDIA CUDA, directml, tensorflow und pytorch.
keywords: WSL, Windows, Windows Subsystem, GPU COMPUTE, GPU Acceleration, NVIDIA, CUDA, directml, tensorflow, pytorch, NVIDIA CUDA Preview, GPU Driver, NVIDIA Container Toolkit, docker
ms.date: 06/17/2020
ms.topic: article
ms.localizationpriority: medium
ms.openlocfilehash: f101022dec534055905b25619a6c4fcee36f3f7d
ms.sourcegitcommit: 031a74801e03a90aed4b34c4fd5bfe964fc30994
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2020
ms.locfileid: "84947410"
---
# <a name="gpu-accelerated-machine-learning-training-in-the-windows-subsystem-for-linux"></a>GPU-beschleunigtes Machine Learning-Training im Windows-Subsystem für Linux

Die Unterstützung für GPU-COMPUTE, das #1 die am meisten angeforderte WSL-Funktion, ist jetzt über das Windows Insider-Programm als Vorschau verfügbar. [Blogbeitrag lesen](https://blogs.windows.com/windowsdeveloper/?p=55781).

## <a name="what-is-gpu-compute"></a>Was ist GPU-Compute?

Die Nutzung der GPU-Beschleunigung für rechenintensive Aufgaben wird im Allgemeinen als "GPU-Compute" bezeichnet. GPU-Computing nutzt die GPU (Graphics Processing Unit) zum Beschleunigen von mathematischen, großen Arbeits Auslastungen und verwendet seine parallele Verarbeitung, um die erforderlichen Berechnungen schneller und in vielen Fällen als die Verwendung einer CPU auszuführen. Diese Parallelisierung ermöglicht deutliche Verbesserungen der Verarbeitungsgeschwindigkeit für diese mathematischen großen Arbeits Auslastungen, bei Ausführung auf einer CPU. Das Trainieren von Machine Learning-Modellen ist ein gutes Beispiel dafür, dass GPU-Compute die Zeit erheblich verkürzen kann, um diese rechenintensive Aufgabe abzuschließen.

## <a name="install-and-set-up"></a>Installieren und Einrichten

Weitere Informationen zur Unterstützung von WSL 2 und zum Einstieg in das Training von Machine Learning-Modellen finden Sie im Leitfaden für die [GPU-Beschleunigung](https://docs.microsoft.com/windows/win32/direct3d12/gpu-accelerated-training) in der directml-Dokumentation. In dieser Anleitung wird Folgendes behandelt:

* Leitfaden für Einsteiger oder Schüler/Studenten zum Einrichten von tensorflow mit directml
* Leitfaden für Fachleute, die mit der Ausführung Ihrer vorhandenen CUDA ml-Workflows beginnen
