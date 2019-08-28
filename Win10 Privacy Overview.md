# Vorwort

Das Projekt ist noch in Arbeit.

</br></br>

# Nutzen

Das Projekt gibt Übersicht über eine datenschutzkonforme Nutzung von Windows 10.

</br></br>

# Microsoft Datenschutzrichtlinien
## OneDrive
Unter folgendem Link ist der Servicevertrag zwischen Anwender und Microsoft geregelt: [Microsoft-Servicevertrag](https://www.microsoft.com/de-de/servicesagreement/)

Auszug bzgl. OneDrive

> b. Soweit dies notwendig ist, um Ihnen und anderen die Dienste bereitzustellen (z. B. durch das Ändern von Größe, 
> Form oder Format Ihrer Inhalte zur besseren Speicherung oder Anzeige), um Sie und die Dienste zu schützen und
> um die Produkte und Dienste von Microsoft zu verbessern, **gewähren Sie Microsoft eine weltweite und
> gebührenfreie Lizenz für geistiges Eigentum zur Verwendung Ihrer Inhalte, z. B. um Kopien Ihrer Inhalte zu erstellen 
> oder Ihre Inhalte aufzubewahren, zu übertragen, neu zu formatieren, mithilfe von Kommunikationswerkzeugen zu verteilen
> und über die Dienste anzuzeigen.**

</br>

## Outlook
Im Folgenden Artikel wird genauer erklärt, dass Microsoft die Anmeldeinformationen abgreift und speichert: [Artikel auf Kuketz-blog.de](https://www.kuketz-blog.de/microsoft-outlook-app-greift-microsoft-die-anmeldedaten-ab/)

> Die offizielle Outlook-App von Microsoft **überträgt** beim Anlegen eines IMAP-Accounts die **kompletten Anmeldedaten an 
> Microsoft.** Fällt soweit nicht auf, allerdings merkte ich in den Serverlogs meines IMAP-Servers, dass sich **IP-Adressen aus > dem Microsoft IP-Bereich mit meinen gültigen Zugangsdaten anmelden und syncen.** Die Outlook-App verbindet sich dann über 
> https mit den Microsoft Servern, **um die E-Mails darzustellen.** Ich denke, mit diesem Verhalten der Outlook-App, gebührt 
> Microsoft ein Platz auf Ihrer Liste von spionierenden E-Mail-Apps.

</br>

## Weitere Tatbestände
Eine Studie im Auftrag des niederländischen Justizministeriums befasste sich ausgiebig mit den übermittelten Telemtriedaten von Office und Windows 10.

- Die Untersuchung der Office Suite ist [hier(PDF)](https://www.rijksoverheid.nl/binaries/rijksoverheid/documenten/rapporten/2019/06/11/data-protection-impact-assessment-windows-10-enterprise/DPIA+Microsoft+Office+365+Online+and+Mobile+SLM+Rijk+23+july.pdf) zu finden. Laut dem Bericht gehen die Daten an das US-Marktforschungsunternehmen Braze.

- Die Untersuchung von Windows 10 mit der Release ID 1809 und 1903 ist [hier(PDF)](https://www.rijksoverheid.nl/binaries/rijksoverheid/documenten/rapporten/2019/06/11/data-protection-impact-assessment-windows-10-enterprise/DPIA+Windows+10+version+1.5+11+June+2019.pdf) zu finden.

> Bei den Windows-Versionen gibt es die Möglichkeit, das Niveau der Diagnosedaten auf "Sicherheit" zu setzen. Diese Einstellung > steht für Windows 10 Enterprise, Windows 10 Mobile und Windows Server zur Verfügung. Dabei werden lediglich **"für den Schutz 
> von Windows und Windows Server erforderliche Informationen"** übertragen. Laut Privacy Company bestehen in diesem Fall keine 
> hohen Datenschutzrisiken, da Microsoft "sehr wenige und keine sensiblen personenbezogenen Daten" verarbeitet. Dennoch 
> bestünden vier niedrigere Risiken, unter anderem durch die **Datenübertragung in die USA** und die **lange Speicherdauer** der Daten. 

(Quelle: [Artikel auf golem.de](https://www.golem.de/news/microsoft-telemetrie-weiter-datenschutzprobleme-mit-office-und-windows-1907-142861.html))

Erneutere Untersuchung [28.08.2019] ergab erneutes Risiko für Windows 10 HOME/PRO Nutzer: [Artikel auf borncity.com](https://www.borncity.com/blog/2019/08/28/windows-10-erneut-im-fokus-der-eu-datenschtzer/)


# Analyse
Unter diesem Namen verbirgt sich ein Datenanalyse Tool von Microsoft, womit Windows 10 Benutzer ihre gesammelten Telemetrie Daten einsehen können. Die gesammelten Daten geben Aufschluss über:

- Verwendete OS Version, Build version und weitere Indikatoren zur Versionierung
- Hardware Informationen (Modell, BIOS version, verbaute Hardware etc.)
- Informationen über verwendete Treiber
- Heruntergeladen Programme und Apps
- Office Version
- Etliche Metadaten zu Windows Updates
- Fehlerberichte
- ...

Diese Liste beschränkt sich lediglich auf die Daten, die uns Microsoft mit dem Tool zugänglich macht. Ich bin mir ziemlich sicher, dass noch viele weitere - wohl auch personenbezogene Daten - an Microsoft übermittelt werden. Und nach einer weile der Benutzung dieses Tools ergaben sich stetig neue Einträge in diesem Tool - fast schon jede 10 Minuten. Es wurde die Stufe "Einfach" genutzt.

<a href="https://www.directupload.net" target="_blank"><img src="https://s17.directupload.net/images/190828/vep835ny.png" title="Kostenlos Bilder und Fotos hochladen"></a>
