---
layout: post
title:  "Erste Schritte mit git"
categories: [ Software ]
image: assets/images/git.jpg   
description: "git."
featured: true
hidden: true
---

Wenn man effizient Software Entwickeln möchte, kommt man um eine Quellcodeverwaltung nicht drum herum. Dies ist in der Regel Git, es wird von verschiedenen Anbietern umgesetzt und selbstverständlich kann auch ein eigener Server mit git ausgestattet werden und als Quellcodeverwaltung dienen. Der bequeme Weg wäre das Nutzen von github oder gitlab.
Doch kurz noch vorab: git ist ein riesiges Thema, es wird hier lediglich der Einstieg betrachtet und wie schnell, mithilfe von git, ein Softwareprojekt sauber entstehen kann.
github und gitlab bieten verschiedene Funktionalitäten, die Basics sind bei beiden Anbietern dieselben.
Dieser Blog wird, beispielsweise, in github.com verwaltet, dies hängt mit dem einfachen Deployment zusammen. Für einige private Projekte, die teilweise aus mehreren Komponenten bestehen, nutze ich gitlab. Gitlab hat einige Vorteile, so schafft es Gitlab das Vereinigen von Software Entwicklung und Operations in einer Anwendung zu gestalten. Außerdem bietet GitLab eine komplexe Nutzerverwaltung.
GitHub bietet Entwicklern die Möglichkeit fremde Projekte zu beobachten, an Diskussionen teilzunehmen oder gar das Projekt zu laden und weiterentwickeln.

Zunächst müsst ihr git auf eurem Computer installieren. Falls ihr Windows-Nutzer seid, könnt ihr es hier herunterladen https://git-scm.com/download/win. Linux-Nutzer geben lediglich diesen Befehl in ihrer Kommandozeile an und folgen in dieser weiteren Anweisungen. Für Mac User wird eine Installation über die XCode CommandLine Tools empfohlen.
In einer Konsole könnt ihr mit dem Befehl git -v die Version überprüfen.
Als Nächstes muss ein gitlab Konto eingerichtet werden, was über die Oberfläche von gitlab.com geschieht.
Sind diese zwei Schritte erledigt, muss es eurem Computer ermöglicht werden sich mit dem gitlab, sicher, also verschlüsselt auszutauschen.
Dies passiert, in dem ein sogenannter ssh key auf dem Computer installiert wird. Öffnet eine Shell eurer Wahl und führt folgenden Befehl aus: ssh-keygen -o. Zunächst wird der Nutzer gefragt, wo er den Key speichern möchte und ob er noch eine besondere Bezeichnung erhalten soll. Bisher hatte ich noch nicht die Notwendigkeit von den Standarteinstellungen abzuweichen.

Ist der Key erzeugt, so wird dieser in gitlab geladen. Loggt euch hierfür zunächst ein, und gelangt über die Einstellung (beim Klick auf euer Profilbild zu finden) in die SSH Key Verwaltung. Sucht euren ssh public key in eurem Verzeichnis, öffnet die Datei und Kopiert den Inhalt in die Textbox. Falls ihr an mehreren Geräten arbeitet, empfiehlt es sich die Keys zu beschriften.

Abschließend würde ich noch gitkraken Installieren. Gitkraken ermöglicht es euch euer GitRepo mit einer Oberfläche zu verwalten. Alternativ kann natürlich die Konsole genutzt werden, diese schreckt aber einige eher ab.

Jetzt sind git, gitlab und gitkraken eingerichtet und es kann mit der Entwicklung begonnen werden. Wie das genau aussieht dazu später mehr...
