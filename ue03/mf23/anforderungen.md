# Anforderungen — Terminplaner für die THM



| Nr. | Anforderung | Stakeholder | Art |
|---|---|---|---|
| A01 | Die Online-Buchung und die personenbezogenen Daten der Studierenden sollen vor unberechtigtem Zugriff geschützt werden. | Studierende | QA |
| A02 | Studierenden sollen zuerst die Lehrenden angezeigt werden, bei denen sie aktuell Vorlesungen besuchen, und anschließend die übrigen Lehrenden der THM. | Studierende | FA |
| A03 | Studierende können gebuchte Termine kurzfristig absagen, müssen jedoch bei einer Absage weniger als 30 Minuten vor dem Termin eine Begründung angeben. | Studierende | FA |
| A04 | Der Terminplaner soll erkennen, welcher Studierende einen Termin zuerst gebucht hat, und eine doppelte Vergabe dieses Termins verhindern. | Studierende | FA |
| A05 | Studierende sollen nach der Anmeldung über ihr THM-Konto Termine buchen können, ohne erneut ihre E-Mail-Adresse, eine TAN oder ihre Matrikelnummer eingeben zu müssen. | Studierende | FA |
| A06 | Die Kommunikation zwischen dem Terminplaner und den Nutzern muss mit TLS 1.3 verschlüsselt werden. | IT-Abteilung der THM | RB |
| A07 | Sprechstundentermine dürfen nur von berechtigten Personen über einen gültigen THM-Zugang gebucht werden. | THM | RB |
| A08 | Der Terminplaner soll während der Vorlesungszeit eine Verfügbarkeit von mindestens 99 % erreichen, wobei planbare Wartungsarbeiten möglichst in den Semesterferien stattfinden sollen. | IT-Abteilung der THM | QA |
| A09 | Die THM stellt einen Server für den Betrieb des Terminplaners bereit. | Rechenzentrum der THM | RB |

## Eine Anforderung, die niemand ausgesprochen hat
A04: Diese Anforderung wurde vermutlich nicht ausdrücklich erwähnt, weil es selbstverständlich ist, dass ein Professor nicht zwei Sprechstundentermine gleichzeitig wahrnehmen kann. Deshalb muss der Terminplaner verhindern, dass derselbe Termin mehrfach vergeben wird.


