# pushbutton

PushButton (ehemals BlinkGame) ist ein kleines Casual Game.

Es basiert aktuell auf einem ubirch#1, der mit einem Taster und einer WS2812 RGB LED verbunden ist. Optional gibt es noch eine Verbindung mit  einem Vibrationsmotor, einem kleinen Piezo-Lautsprecher und einem zweiten Taster (Mode-Umschaltung).

In seiner einfachsten Version beleuchtet für eine bestimmte Zeit (3-8 Sekunden) die LED blau auf und erlischt dann wieder. Nun wartet das Spiel darauf, dass man die LED durch Drücken des Tasters wieder zum Leuchten bringt und zwar möglichst genau so lange, wie sie vorher geleuchtet hat. Schafft man es, die Richtzeit auf 0,3 Sekunden genau zu treffen, gilt die Runde als gewonnen und die LED leuchtet grün auf, schafft man es nicht, leuchtet sie rot. Nach 2 bis 3 Sekunden Pause startet die nächste Runde.

Die Ergennisse der Spiele werden alle 10 Spiele mit der unique-ID des Devices auf den ubirch-Server hochgeladen.


Spielvariante 1: Der Vibrationsmotor vibriert ein paar mal kurz und danach lang. Sobald man glaubt, das er lang vibriert, muss man den Button drücken und es wird die Reaktionszeit gemessen.

Spielvariante 2: Der Piezolautsprecher gibt einen Ton aus, der bei Frequenz X beginnt und auf Frequent Y ansteigt oder abfällt. Danach muss man den Taster drücken und so lange halten, bis man glaubt den richtigen Ton erreicht zu haben. Alternativ wird als Referenz nur eine Frequenz ausgegeben, die man dann treffen muss. Hier wird dann der Frequenzunterschied zur Bewertung benutzt.

Momentan werden die Spiele alle zufällig on-the-fly erzeugt. Es gibt die Idee, dass sich das PushButton-Game einmal am Tag Spieldaten herunterlädt und so eine exaktere Vergleichbarkeit von Ergebnissen ermöglicht.

