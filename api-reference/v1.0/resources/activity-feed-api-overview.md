# <a name="use-the-activity-feed-rest-api"></a>Verwenden Sie die Aktivitätsfeed-REST-API

Sie können den Aktivitätsfeed-API in Microsoft Graph benutzen, um die Geräte und Plattformen übergreifenden Aktivitäten eines Benutzers fortzusetzen. Die Aktivitätsfeed-API-Anforderungen werden im Auftrag eines Benutzers über [delegierte Berechtigungen](../../../concepts/permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions) und die [Benutzeraktivitätsberechtigung](../../../concepts/permissions_reference.md) ausgeführt, die entweder mit persönlichen oder beruflichen und schulischen Konten verwendet werden können. 

Die Benutzeraktivitäten werden von der Ressource [Aktivität](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity) dargestellt und sind in einem zeitbasierten Feed, der durch die Sammlung mich/Aktivitäten dargestellt wird, organisiert. 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>Was macht eine großartige Benutzer-Aktivität aus?

Bei Nutzeraktivitäten werden nicht nur Apps gestartet, sondern auch Deep Links zu bestimmten Inhalten in Ihrer App. Die Benutzeraktivitäten, die Sie erstellen, können nicht nur in Ihrer eigenen App verwendet werden, sondern werden auch in der Cortana und Windows-Timeline angezeigt. Dies führt zu mehr App-Reengagements und erleichtert es Ihren Nutzern, Ihre App weiterhin auf mehreren Geräten zu verwenden.  

### <a name="what-should-become-an-activity"></a>Was sollte eine Aktivität werden? 

Da jede App verschieden ist, liegt es an jedem App-Entwickler, die beste Möglichkeit zum Zuordnen von Aktionen innerhalb der Anwendung zu Benutzeraktivitäten zu verstehen. Beispielsweise können Spiele für jede Kampagne eine Aktivität erstellen, während die Erstellung von Dokumenten-Apps möglicherweise eine Aktivität für jedes einzigartige Dokument erstellen, und Branchen-Apps können für jeden Workflow eine Aktivität erstellen. 

Wenden Sie die folgenden Richtlinien an, wie Sie in Ihren App-Aktivitäten definiert sind:

**DO:** Tragen Sie eine einzelne Aktivität für eine Gruppe von verwandten Benutzeraktionen ein. Wenn Ihre Anwendung bei einer Sequenz von verwandten Inhalten verwendet wird, ist es wahrscheinlich sinnvoll, eine einzelne Aktivität für die gesamte Sitzung aufzuzeichnen.  

*Wiedergabeliste Szenarien:* Dies ist besonders relevant für Musik-Wiedergabelisten oder TV-Programme – eine Aktivität einzelner Benutzer kann aktualisiert werden, um Ihren Fortschritt anzuzeigen. In diesem Fall werden Sie eine einzelne Benutzeraktivität mit mehreren [Punkten aus Ereignisprotokollen](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_historyitem) erhalten, die über mehrere Tage oder Wochen hinweg Zeiträume des Engagements darstellen.  

**DO:** Speichern von Benutzerdaten in die Cloud. Wenn Sie geräteübergreifende Aktivitäten unterstützen möchten, müssen Sie sicherstellen, dass der für die erneute Aktivierung dieser Aktivität erforderliche Inhalt an einem Cloud-Speicherort gespeichert wird. Wenn Sie beispielsweise eine Aktivität jedes Mal veröffentlichen, wenn ein Benutzer ein Dokument bearbeitet, sollte das Dokument in der Cloud gespeichert werden und nicht lokal auf dem Gerät des Benutzers, um geräteübergreifendes Reengagement zu ermöglichen.  

**TUN SIE NICHT:** Eine Benutzeraktivität für Aktionen erstellen, die Benutzer nicht benötigen, um zukünftig fortzusetzen. Wenn Ihre Anwendung zum Ausführen einfacher, einmaliger Vorgänge verwendet wird, deren Status für die zukünftige Verfolgung nicht beibehalten wird, brauchen Sie wahrscheinlich keine Benutzeraktivität zu schreiben. 

Um Klarheit zu schaffen: Obwohl die Benutzeraktivitäten in der Windows-Timeline angezeigt werden, dient dies nicht als Werkzeug zur Versionsverwaltung – das Auswählen einer dokumentbasierten Aktivität sollte immer die neueste Version dieses Dokuments (einschließlich Änderungen, die von einem anderen Benutzer vorgenommen wurden) anzeigen.

**DO NOT:** Eine Benutzeraktivität für Aktionen erstellen, die von *anderen Benutzern abgeschlossen wurde*. Wenn jemand dem Benutzer eine Nachricht sendet oder den Benutzer innerhalb Ihrer App @erwähnt, sollte keine neue Aktivität geschrieben werden. Diese Interaktionen erfolgen besser durch das Auftauchen von Benachrichtigungen.  

*Szenarien der Zusammenarbeit:* Wenn mehrere Personen an der gleichen Aktivität (beispielsweise an einem Word-Dokument) arbeiten, wird es Fälle geben, in denen ein anderer Benutzer Änderungen an dem Dokument vorgenommen hat, nachdem Sie es zuletzt bearbeitet haben. In diesem Fall möchten App-Entwickler die visuellen Elemente in der Aktivität aktualisieren, um die Änderungen an dem Dokument zu reflektieren. Dazu aktualisiert die App möglicherweise die vorhandene Aktivität, ohne ein neues Verlaufselement zu erstellen. 

>**Hinweis:** Wenn Sie Aktivitäten für eine Webanwendung veröffentlichen, ist es wichtig, sowohl eine `activationURL` einzubeziehen als auch eine `fallbackURL` für jede Ihrer Aktivitäten. Die Aktivitäten bringen den Benutzer zu Ihrer App zurück, wie es bei Microsoft-Erfahrungen wie Windows-Timeline erwartet wird. 

## <a name="app-interaction-patterns-and-user-activities"></a>App-Interaktionsmuster und die Benutzeraktivitäten 
Die Benutzeraktivitäten, die Sie erstellen, variieren basierend auf dem Interaktionsmuster Ihrer App. Während jede App unterschiedlich ist, werden die meisten zu einem der folgenden Interaktionsmuster gehören: 

* **Dokumentbasierte Apps** – Erstellen einer Aktivität pro Dokument mit mindestens einem oder mehreren Ereignisprotokollen, die Zeiträume der Nutzung anzeigen. Es ist wichtig, Ihre Aktivitäten-Karte zu aktualisieren, da Änderungen an dem Dokument erfolgten. 
* **Medien-Wiedergabe Apps** – Erstellen einer Aktivität pro logischer Gruppierung von Inhalten wie eine Wiedergabeliste, ein Programm oder eigenständige Inhalte. 
* **Spiele** – Erstellen Sie eine Aktivität für jedes gespeicherte Spiel oder jede Welt. Wenn Ihr Spiel nur eine einzelne Sequenz von Ebenen unterstützt, können Sie die gleiche Aktivität im Laufe der Zeit schreiben, obwohl Sie vielleicht Ihre Karte zum Anzeigen Ihres aktuellen Status oder Ihrer Erfolge aktualisieren möchten. 
* **Utility-Apps** – <g id = "3521"> - Wenn in Ihrer App nichts vorhanden ist, das die Nutzer fortsetzen möchten, sollten Sie keine Aktivitäten veröffentlichen Ein gutes Beispiel ist eine einfache App für einen Einzelzweck wie der Taschenrechner. 
* **Branchen-Apps** – Viele Apps gibt es zum Verwalten von einfachen Aufgaben oder Workflows. Erstellen Sie eine Aktivität für jeden separaten Workflow über Ihre App. Beispielsweise wäre jede Spesenabrechnung eine separate-Aktivität, da Sie möglicherweise auf diese Aktivität klicken werden, um festzustellen, ob sie genehmigt wurde.

*Einige komplexe Apps enthalten mehrere Interaktionsmuster. Unter Umständen möchten Sie verschiedenen Mustern zur Erstellung von Benutzeraktivitäten für verschiedene Szenarien folgen, die von Ihrer App behandelt werden.*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich die [Aktivitäten-Ressource](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/projectrome_activity) an und definieren Sie Ihre App-Aktivitäten, damit Sie Benutzern helfen, wichtige Aufgaben fortsetzen zu können.
- Erkunden Sie die [adaptiven Karten-Beispiele,](http://adaptivecards.io/samples/) Beispiele für Ideen, um Ihre Aktivitäten **hervorstechen zu lassen** .  
- Probieren Sie die API im [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer) aus.

**Sie möchten noch mehr erfahren?** 
- Finden Sie unter [wie Microsoft Erfahrungen Aktivitäten verwendet](https://channel9.msdn.com/events/Build/2017/B8108).
- Informieren Sie sich über [die Aktivitätsfeed API und fahren Sie fort, wo ich aufgehört habe](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
