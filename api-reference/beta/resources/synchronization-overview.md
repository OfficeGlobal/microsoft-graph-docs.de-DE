---
title: Azure AD-Synchronisierung API (Übersicht)
description: ') können Sie die Erstellung automatisieren Wartung und Entfernen von Identitäten in cloud (Software als Dienst oder SaaS) Anwendungen wie Ablage, Vertriebs, ServiceNow und vieles mehr. Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:'
ms.openlocfilehash: ff3acb00801c9b04b8257345b06100297e11710c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064792"
---
# <a name="azure-ad-synchronization-api-overview"></a>Azure AD-Synchronisierung API (Übersicht)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Azure Active Directory (AD Azure) Identität Synchronisierung (auch als "Bereitstellung" bezeichnet) können Sie die Erstellung, Wartung und Entfernen von Identitäten in der Cloud (Software als Dienst oder SaaS) automatisieren Applications wie Ablage, Vertriebs, ServiceNow, und vieles mehr. Die Synchronisierung-APIs können in Microsoft Graph Sie programmgesteuert verwalten Identität Synchronisierung einschließlich:

- Erstellen Sie, starten Sie und beenden Sie der Aufträge für die Synchronisierung
- Vornehmen von Änderungen an der Synchronisierungsschema für Aufträge
- Überprüfen Sie den aktuellen Synchronisierungsstatus 

Weitere Informationen zur Synchronisierung in Azure Active Directory finden Sie unter:

* [Automatisieren der Benutzer bereitstellen und entziehen für SaaS Clientanwendungen mit Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Verwalten von Benutzerkonto für Enterprise-apps im Azure-Portal-Bereitstellung](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Sie können auch die API im [Graph-Explorer](https://developer.microsoft.com/graph/graph-explorer) in einer Beispiel-Mandanten oder Ihre eigene Mandanten versuchen.

## <a name="synchronization-job"></a>Synchronisierungsauftrag

Aufträge für die Synchronisierung ausführen Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis. Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten. Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.

Weitere Informationen finden Sie unter [Synchronisierungsauftrag](synchronization-synchronizationjob.md).

## <a name="synchronization-schema"></a>Synchronisierungsschema

Das Synchronisierungsschema definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll. Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag. Sie werden in der Regel anpassen einiger [Attribut Zuordnungen](synchronization-attributemapping.md)oder Hinzufügen eines [Gültigkeitsbereichs Filter](synchronization-filter.md) , um nur die Objekte zu synchronisieren, die eine bestimmte Bedingung erfüllen.

Das Synchronisierungsschema umfasst die folgenden Komponenten:

- Directory-Definitionen
- Synchronisierungsregeln
- Objekt-Zuordnungen

Weitere Informationen finden Sie unter [Synchronisierungsschema](synchronization-synchronizationschema.md).

## <a name="synchronization-template"></a>Synchronisierung-Vorlage

Die Synchronisierung Vorlage enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung. Diese Einstellungen (vor allem [Synchronisierungsschema](synchronization-synchronizationschema.md)) werden standardmäßig für alle [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet werden, die auf der Vorlage basiert. Vorlagen, die vom Anwendungsentwickler festgelegt werden.

Weitere Informationen finden Sie unter [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md).

## <a name="working-with-the-synchronization-api"></a>Arbeiten mit der API-Synchronisierung

Arbeiten mit Synchronisierung umfasst API in erster Linie den Zugriff auf die [SynchronizationJob](synchronization-synchronizationjob.md) und [SynchronizationSchema](synchronization-synchronizationschema.md) Ressourcen. Damit die Ressource [SynchronizationJob](synchronization-synchronizationjob.md) ermittelt wird, müssen Sie die ID des Service principal-Objekts wissen, zu der der Synchronisierungsauftrag gehört. Die folgenden Beispiele zeigen, wie die Ressourcen **SynchronizationJob** und **SynchronizationSchema** entwickelt.

### <a name="authorization"></a>Authorization

Die Azure AD-Synchronisierung API verwendet OAuth 2.0 für die Autorisierung. Vor der Durchführung von alle Anforderungen an die API, müssen Sie ein Zugriffstoken abzurufen. Weitere Informationen finden Sie unter [Get Access tokens Microsoft Graph aufrufen](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Um den Zugriff auf Ressourcen Synchronisierung benötigt Ihre Anwendung Directory.ReadWrite.All Berechtigungen. Weitere Informationen finden Sie unter [Directory-Berechtigungen](/graph/permissions-reference#directory-permissions).

### <a name="find-the-service-principal-object-by-display-name"></a>Hier finden Sie das principal-Objekt nach Anzeigename

Im folgenden Beispiel wird gezeigt, wie Service principal-Objekt nach dem Anzeigenamen zu suchen.

**Anforderung** 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

**Response**

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a>Hier finden Sie das principal-Objekt von app-ID

Das folgende Beispiel zeigt, wie Sie finden das principal-Objekt nach app-ID.

**Anforderung** 
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**Antwort**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a>Liste der vorhandenen Aufträge für die Synchronisierung

Das folgende Beispiel veranschaulicht das Auflisten der vorhandenen Aufträge für die Synchronisierung.

**Anforderung**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**Antwort**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a>Erste Synchronisierung Auftragsstatus
Im folgende Beispiel wird das Abrufen des Status eines Auftrags zur Synchronisierung veranschaulicht.

**Anforderung**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**Antwort**
<!-- { "blockType": "ignored" } -->
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a>Erste Synchronisierungsschema
Im folgende Beispiel wird das Abrufen des Synchronisierungsschemas veranschaulicht.

**Anforderung**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**Antwort**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>Siehe auch

* [Konfigurieren der Synchronisierung mit Verzeichnis Extension-Attribute](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute](../resources/synchronization-configure-with-custom-target-attributes.md)



