---
layout: post
title:  "Erste Schritte mit Git"
categories: [ Software ]
image: assets/images/git.jpg   
description: "Git."
featured: true
hidden: true
---

Wenn man effizient und entwicklerfreundlich Software Entwickeln möchte, kommt man um eine Quellcodeverwaltung nicht drum herum. Dies ist in der Regel Git, es wird von verschiedenen Anbietern umgesetzt und selbstverständlich kann auch ein eigener Server mit Git ausgestattet werden und als Quellcodeverwaltung dienen.  
Git ermöglicht dem Entwickler seinen Code zu verwalten, zu älteren Zuständen zu wechseln oder von einer Codebasis aus verschiedene Features gleichzeitig zu lösen. Der bequeme Weg wäre das Nutzen von [GitHub][2] oder [GitLab][1].  
Doch kurz noch vorab: Git ist ein riesiges Thema, es wird hier lediglich der Einstieg betrachtet und wie schnell, mithilfe von Git, ein Softwareprojekt sauber entstehen kann.
GitHub und GitLab bieten verschiedene Funktionalitäten, die Basics sind bei beiden Anbietern dieselben.  
Dieser Blog wird, beispielsweise, in GitHub verwaltet, dies hängt mit dem einfachen Deployment zusammen. Für einige private Projekte, die teilweise aus mehreren Komponenten bestehen, nutze ich GitLab. Gitlab hat einige Vorteile, so schafft es GitLab das Vereinigen von Software Entwicklung und Operations in einer Anwendung zu gestalten. Außerdem bietet GitLab eine komplexe Nutzerverwaltung.
Wohingenen GitHub Entwicklern die Möglichkeit bietet fremde Projekte zu beobachten, an Diskussionen teilzunehmen oder gar das Projekt zu laden und weiterentwickeln.

****

Zunächst müsst ihr Git auf eurem Computer installieren. Falls ihr Windows-Nutzer seid, könnt ihr es hier [herunterladen][3] . Linux-Nutzer geben lediglich diesen Befehl in ihrer Kommandozeile ein und folgen in dieser weiteren Anweisungen. Für Mac User wird eine Installation über die XCode CommandLine Tools empfohlen.  
In einer Konsole könnt ihr, Betriebssystem unabhängig, mit dem Befehl Git -v die Version, beziehungsweise den Erfolg der Installation prüfen.  
Als Nächstes muss ein GitLab Konto eingerichtet werden, was über die Oberfläche von [GitLab][4] geschieht.  
Sind diese zwei Schritte erledigt, muss es eurem Computer ermöglicht werden sich mit dem GitLab, sicher, also verschlüsselt auszutauschen.
Dies passiert, in dem ein sogenannter ssh key auf dem Computer installiert wird. Öffnet eine Shell eurer Wahl und führt folgenden Befehl aus:  
`ssh-keygen -o`  
Während der Befehl ausgeführt wird, wird der Nutzer nach einem spezifischen Speicherort gefragt und nach einer Bennenung des Keys. Diese Eingaben sind jedoch nicht Notwendig und können ungefüllt bleiben. Falls kein konkreter Speicherort angegeben wird, findet ihr den SSH-Key `asda` hier.

****

Ist der Key erzeugt, so muss dieser in GitLab hinterlegt werden. Loggt euch hierfür zunächst ein, und gelangt über die Einstellung (beim Klick auf euer Profilbild zu finden) in die SSH Key Verwaltung oder gelangt über diesen [Link][4] direkt dorthin. Sucht euren ssh public key in eurem Verzeichnis, öffnet die Datei und Kopiert den Inhalt in die Textbox. Falls ihr an mehreren Geräten arbeitet, empfiehlt es sich die Keys zu beschriften.

****

Abschließend würde ich noch GitKraken Installieren. GitKraken ermöglicht es euch euer GitRepo mit einer Oberfläche zu verwalten. Alternativ kann natürlich die Konsole genutzt werden, diese schreckt aber einige eher ab.

Jetzt sind Git, GitLab und GitKraken eingerichtet und es kann mit der Entwicklung begonnen werden. Wie das genau aussieht dazu später mehr...



[1]:https://gitlab.com/
[2]:https://github.com/
[3]:https://git-scm.com/download/win
[4]:https://gitlab.com/users/sign_up
[5]:https://gitlab.com/profile/keys
