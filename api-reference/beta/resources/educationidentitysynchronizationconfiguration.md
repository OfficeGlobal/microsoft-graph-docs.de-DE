    ---
Titel: "EducationIdentitySynchronizationConfiguration Ressourcentyp" Beschreibung: "abstrakte Basisklasse für alle Schule Daten Profil Identität Synchronisierung Konfigurationen. Abgeleiteten Klassen definieren Sie das Verhalten für das Synchronisieren von Identitäten. Im folgenden werden die abgeleiteten Typen."
Autor: "Mmast Msft" Localization_priority: normalen ms.prod: "Education"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>Ressourcentyp educationIdentitySynchronizationConfiguration

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abstrakte Basisklasse für alle Schule Daten Profil Identität Synchronisierung Konfigurationen. Abgeleiteten Klassen definieren Sie das Verhalten für das Synchronisieren von Identitäten. Im folgenden werden die abgeleiteten Typen.

## <a name="derived-types"></a>Abgeleitete Typen
| Typ | Beschreibung |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Verwenden Sie diesen Typ zu vorhandenen Benutzerkonten in Azure Active Directory (AD Azure) übereinstimmen. |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Verwenden Sie diesen Typ in Azure Active Directory neue Benutzerkonten erstellen. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
