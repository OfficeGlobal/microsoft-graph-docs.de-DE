---
title: domain-Ressourcentyp
description: Stellt eine Domäne dar, die einem Mandanten zugewiesen ist.
ms.openlocfilehash: c3a130f00afd3c9136b8ae8238f37cf99d5a6fc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016513"
---
# <a name="domain-resource-type"></a>domain-Ressourcentyp

Stellt eine Domäne dar, die einem Mandanten zugewiesen ist.

Verwenden Sie Domänenvorgänge, um Domänen einem Mandanten zuzuweisen, den Besitz von Domänen zu überprüfen und unterstützte Dienste zu konfigurieren.  Mithilfe von Domänenvorgängen können Registrierungsstellen die Domänenzuweisung für Dienste wie Office 365 automatisieren. Im Rahmen der Domänenanmeldung kann eine Registrierungsstelle beispielsweise eine Vanity-Domäne für E-Mails, Websites, Authentifizierung usw. aktivieren.

So ordnen Sie eine Domäne einem Mandanten zu:

1. [Ordnen Sie](../api/domain-post-domains.md) dem Mandanten eine Domäne zu.

2. [Rufen Sie](../api/domain-list-verificationdnsrecords.md) die Domänenüberprüfungseinträge ab. Fügen Sie die Details des Überprüfungsdatensatzes mithilfe der Domänenregistrierungsstelle oder der DNS-Serverkonfiguration der Zonendatei der Domäne hinzu.

3. [Überprüfen Sie](../api/domain-verify.md) den Besitz der Domäne. Dadurch wird die Domäne überprüft und die *IsVerified*-Eigenschaft auf *true* festgelegt.

4. [Geben Sie](../api/domain-update.md) die unterstützten Dienste an, die Sie mit der Domäne verwenden möchten.

5. [Konfigurieren Sie](../api/domain-list-serviceconfigurationrecords.md) unterstützte Dienste, indem Sie eine Liste von Datensätzen abrufen, die zum Aktivieren von Diensten für die Domäne erforderlich sind. Fügen Sie die Details des Konfigurationsdatensatzes mithilfe der Domänenregistrierungsstelle oder der DNS-Serverkonfiguration der Zonendatei der Domäne hinzu.

## <a name="methods"></a>Methoden

| Methode   | Rückgabetyp |Beschreibung|
|:---------------|:--------|:----------|
|[Domäne abrufen](../api/domain-get.md) | [Domäne](domain.md) | Dient zum Lesen der Eigenschaften und der Beziehungen eines Domänenobjekts.|
|[Domäne erstellen](../api/domain-post-domains.md) | [Domäne](domain.md) | Fügt eine Domäne zum Mandanten hinzu. |
|[domainNameReference auflisten](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen einer Liste von Verzeichnisobjekten mit einem Verweis auf die Domäne.|
|[serviceConfigurationRecords auflisten](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md)-Sammlung|  Dient zum Abrufen einer von Domänen-DNS-Einträgen für die Domänenkonfiguration.|
|[verificationDnsRecords auflisten](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md)-Sammlung|  Dient zum Abrufen einer von Domänen-DNS-Einträgen für die Domänenüberprüfung.|
|[Domäne aktualisieren](../api/domain-update.md) | [Domäne](domain.md) |Dient zum Aktualisieren einer Domäne.|
|[Domäne löschen](../api/domain-delete.md) | Keine |Dient zum Löschen einer Domäne.|
|[ForceDelete Domäne](../api/domain-forcedelete.md)|Keines|Löscht eine Domäne mithilfe eines asynchronen Vorgangs.|
|[Domäne überprüfen](../api/domain-verify.md)|[Domäne](domain.md)|Überprüft den Besitz der Domäne.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
|authenticationType|String| Gibt den konfigurierten Authentifizierungstyp für die Domäne an. Der Wert ist entweder *Verwaltet* oder *Verbund*.<br> *Verwaltet* gibt eine cloudverwaltete Domäne an, bei der Azure AD die Benutzerauthentifizierung ausführt.<br>*Verbund* gibt an, dass die Authentifizierung im Verbund mit einem Identitätsanbieter steht, z. B. das lokale Active Directory des Mandanten über Active Directory-Verbunddienste. Lässt keine Nullwerte zu. |
|availabilityStatus|String| Diese Eigenschaft ist immer null, außer wenn die Aktion [verify](../api/domain-verify.md) verwendet wird. Wenn die Aktion [verify](../api/domain-verify.md) verwendet wird, wird in der Antwort eine **Domänen**entität zurückgegeben. Die Eigenschaft **availabilityStatus** der **Domänen**entität in der Antwort ist entweder *AvailableImmediately* oder *EmailVerifiedDomainTakeoverScheduled*.|
|id|String| Der vollqualifizierte Name der Domäne. Schlüssel, unveränderlich, lässt keine Nullwerte zu, eindeutig |
|isAdminManaged|Boolescher Wert| Der Wert der Eigenschaft ist „false“, wenn die DNS-Datensatzverwaltung der Domäne an Office 365 delegiert wurde. Andernfalls ist der Wert „true“. Lässt keine Nullwerte zu. |
|isDefault|Boolescher Wert| „True“, wenn dies die Standarddomäne ist, die für die Benutzererstellung verwendet wird. Es gibt nur eine Standarddomäne pro Unternehmen. Lässt keine Nullwerte zu. |
|isInitial|Boolescher Wert| „True“, wenn dies die erste Domäne ist, die von Microsoft Online Services (companyname.onmicrosoft.com) erstellt wird. Es gibt nur eine anfängliche Domäne pro Unternehmen. Lässt keine Nullwerte zu. |
|isRoot|Boolescher Wert| „True“, wenn die Domäne eine überprüfte Stammdomäne ist. Andernfalls „false“, wenn die Domäne eine Unterdomäne oder ungeprüft ist. Lässt keine Nullwerte zu. |
|isVerified|Boolescher Wert| „True“, wenn die Domänenbesitzüberprüfung für die Domäne abgeschlossen ist. Lässt keine Nullwerte zu. |
|supportedServices|String-Sammlung| Die der Domäne zugewiesenen Funktionen.<br><br>Kann 0, 1 oder mehrere der folgenden Werte umfassen: *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*<br><br> Zu den Werten, die Sie mithilfe der Graph-API hinzufügen/entfernen können, gehören: *Email*, *OfficeCommunicationsOnline*, *Yammer*<br>Lässt keine Nullwerte zu.|
|Status|[domainState](domainstate.md)| Status von asynchronen Vorgängen, die für die Domäne geplant sind. |

## <a name="relationships"></a>Beziehungen

Beziehungen zwischen einer Domäne und anderen Objekten im Verzeichnis, z. B. die Überprüfungsdatensätze und Dienstkonfigurationsdatensätze, die über Navigationseigenschaften verfügbar gemacht werden. Sie können diese Beziehungen lesen, indem Sie auf diese Navigationseigenschaften in Ihren Anforderungen abzielen.

| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md)-Sammlung| DNS-Einträge, die der Kunde der Zonendatei der Domäne hinzufügt, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann.<br>Schreibgeschützt. Lässt Nullwerte zu. |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md)-Sammlung| DNS-Einträge, die der Kunde der DNS-Zonendatei der Domäne hinzufügt, bevor die Domänenbesitzüberprüfung mit Azure AD abgeschlossen werden kann.<br>Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->