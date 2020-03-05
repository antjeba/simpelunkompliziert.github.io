---
layout: post
title:  "Erste Schritte mit git"
categories: [ Software ] [git]
image: assets/images/co2-sparen.jpg   
description: "CO2 sparen im Haushalt."
featured: true
---

Wenn man Software Entwickeln möchte, kommt man um eine Quellcodeverwaltung nicht drum herum. Was früher svn war ist heute git. Git wird von verschiedenen Anbietern umgesetzt. Eine der bekanntesten Plattformen sind github.com und gitlab.com .
Dieser Blog wird in github.com verwaltet, dies hängt mit dem einfachen Deployment zusammen. Für einige private Projekte, die teilweise aus mehreren Komponenten bestehen, nutze ich github. Github hat einige Vorteile, was das Builden und Deployen angeht (sicherlich noch weitere).
Nun aber von Anfang an.

Zunächst müsst ihr git auf eurem Computer installieren. Falls ihr Windows-Nutzer seid, könnt ihr es hier runterladen https://git-scm.com/download/win. Linux-Nutzer geben lediglich diesen Befehl in ihrer Kommandozeile an und folgen in dieser weiteren Anweisungen. Für Mac User wird eine Installation über die XCode CommandLine Tools empfohlen.
In einer Konsole könnt ihr mit dem Befehl git -v die Version überprüfen.
Als nächstes muss ein gitlab Konto eingerichtet werden, was über die Oberfläche von gitlab.com geschieht.
Sind diese zwei Schritte erledigt, muss es eurem Computer ermöglicht werden sich mit dem gitlab, sicher, also verschlüsselt auszutauschen.
Dies passiert, in dem ein sogenannter ssh key auf dem Computer installiert wird. Öffnet eine Shell eurer Wahl und führt folgenden Befehl aus: ssh-keygen -o . Zunächst wird der Nutzer gefragt wo er den Key speichern möchte und ob er noch eine besondere Bezeichnung erhalten soll. Bisher hatte ich noch nicht die Notwendigkeit von den Standarteinstellungen abzuweichen.

Ist der Key erzeugt, so wird dieser in gitlab geladen. Loggt euch hierfür zunächst ein, und gelangt über die Einstellung (beim Klick auf euer Profilbild zu finden) in die SSH Key Verwaltung. Sucht euren ssh public key in eurem Verzeichnis, öffnet die Datei und Kopiert den Inhalt in die Textbox. Falls ihr an mehreren Geräten arbeitet, empfiehlt es sich die Keys zu beschriften.

Abschließend würde ich noch gitkraken Installieren. Gitkraken ermöglicht es euch euer GitRepo mit einer Oberfläche zu verwalten. Alternativ kann natürlich die Konsole genutzt werden, diese schreckt aber einige eher ab.

Jetzt sind git, gitlab und gitkraken eingerichtet und es kann mit der Entwicklung begonnen werden. Wie das genau aussieht dazu später mehr...





















https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
