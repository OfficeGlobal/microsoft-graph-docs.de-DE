---
title: Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute
description: Sie können das Synchronisierungsschema, um benutzerdefinierte Attribute enthalten, die in das Zielverzeichnis definiert sind, anpassen. In diesem Artikel wird beschrieben, wie ein Abonnement Vertriebs anpassen, indem Sie ein neues Feld namens hinzufügen `officeCode`. Richten Sie die Synchronisierung von Azure Active Directory (AD Azure) zu Vertriebs, und für jeden Benutzer, füllen Sie die `officeCode` Feld Vertriebs mit dem Wert aus der `extensionAttribute10` in Azure AD-Feld.
localization_priority: Normal
ms.openlocfilehash: 3a7612682794109a5f94318304c8a8898764ccb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806755"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a>Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können das Synchronisierungsschema, um benutzerdefinierte Attribute enthalten, die in das Zielverzeichnis definiert sind, anpassen. In diesem Artikel wird beschrieben, wie ein Abonnement Vertriebs anpassen, indem Sie ein neues Feld namens hinzufügen `officeCode`. Richten Sie die Synchronisierung von Azure Active Directory (AD Azure) zu Vertriebs, und für jeden Benutzer, füllen Sie die `officeCode` Feld Vertriebs mit dem Wert aus der `extensionAttribute10` in Azure AD-Feld.

In diesem Artikel wird davon ausgegangen, dass Sie bereits eine Anwendung hinzugefügt haben, die von der Synchronisierung Ihres Mandanten über das [Portal Azure](https://portal.azure.com)unterstützt, dass Sie den Anzeigenamen der Anwendung kennen und Sie Authentifizierungstoken für Microsoft Graph verfügen. Informationen dazu, wie Sie das Autorisierungstoken erhalten möchten finden Sie unter [Get-Zugriff zum Aufrufen von Microsoft Graph-Token](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Hier finden Sie das principal-Objekt nach Anzeigename

Im folgenden Beispiel wird veranschaulicht, wie ein Service principal-Objekt mit dem Anzeigenamen Vertriebs suchen.

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(id,appId,displayName)",
    "value": [
    {
        "id": "167e33e9-f80e-490e-b4d8-698d4a80fb3e",
        "appId": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
        "displayName": "Salesforce"
    },
    {
        "id": "8cbbb70b-7290-42da-83ee-89fa3517a977",
        "appId": "b0f2e3b1-fe31-4658-b216-44dcaeabb63a",
        "displayName": "salesforce 1"
    },
    {
        "id": "60443998-8cf7-4e61-b05c-a53b658cb5e1",
        "appId": "79079396-c301-405d-900f-e2e0c2439a90",
        "displayName": "Salesforce Sandbox"
    }
    ]
}
```

Die `{servicePrincipalId}` ist `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Synchronisierungsaufträge im Zusammenhang mit den Dienstprinzipal auflisten 

Das folgende Beispiel veranschaulicht das Abrufen der `jobId` , die Sie benötigen entwickelt. Im Allgemeinen gibt die Antwort nur einen Auftrag zurück.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('60443998-8cf7-4e61-b05c-a53b658cb5e1')/synchronization/jobs",
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {},
            "status": {}
    }
    ]
}
```

Die `{jobId}` ist `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.


## <a name="get-the-synchronization-schema"></a>Abrufen des Synchronisierungsschemas
Im folgenden Beispiel wird gezeigt, wie das Synchronisierungsschema abgerufen.

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
  "directories": [
        {
              "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
              "name": "Azure Active Directory",
              "objects": [
                {
                    "attributes": [
                        {
                          "anchor": true,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "objectId",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        },
                        {
                          "anchor": false,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "streetAddress",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        }
                    ],
                    "name": "User"
                }
             ]
        },
        {
              "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
              "name": "salesforce.com",
              "objects": []
        }
  ],
 "synchronizationRules": [
        {
          "editable": true,
          "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
          "name": "USER_OUTBOUND_USER",
          "objectMappings": [
                {
                    "attributeMappings": [
                            {
                              "defaultValue": "True",
                              "exportMissingReferences": false,
                              "flowBehavior": "FlowWhenChanged",
                              "flowType": "Always",
                              "matchingPriority": 0,
                              "source": {
                                "expression": "Not([IsSoftDeleted])",
                                "name": "Not",
                                "parameters": [
                                  {
                                    "key": "source",
                                    "value": {
                                      "expression": "[IsSoftDeleted]",
                                      "name": "IsSoftDeleted",
                                      "parameters": [],
                                      "type": "Attribute"
                                    }
                                  }
                                ],
                                "type": "Function"
                              },
                              "targetAttributeName": "IsActive"
                            }
                     ],
                    "enabled": true,
                    "flowTypes": "Add, Update, Delete",
                    "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
            }]
        }]
}
```

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a>Fügen Sie eine Definition für das Attribut OfficeCode und eine Zuordnung zwischen Attributen

Verwenden Sie, um eine nur-Text-Editor Ihrer Wahl (beispielsweise [Editor ++](https://notepad-plus-plus.org/) oder [JSON Editor Online](https://www.jsoneditoronline.org/)):

1. Hinzufügen einer [Attributdefinition](synchronization-attributedefinition.md) für die `officeCode` Attribut. 

    - Klicken Sie unter Verzeichnisse Hier finden Sie das Verzeichnis mit dem Namen "Salesforce.com", und klicken Sie in das Objekt-Array, suchen Sie der eine benannte **Benutzer**.
    - Fügen Sie das neue Attribut zur Liste der Name und Typ, angeben, wie im folgenden Beispiel dargestellt.

2. Hinzufügen einer [Zuordnung zwischen Attributen](synchronization-attributemapping.md) zwischen `officeCode` und `extensionAttribute10`.

    - Finden Sie unter [SynchronizationRules](synchronization-synchronizationrule.md), die Regel, die als Quellverzeichnis und Salesforce.com als das Zielverzeichnis Azure AD angibt (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).
    - Suchen Sie in der [ObjectMappings](synchronization-objectmapping.md) der Regel, die Zuordnung zwischen Benutzern (`"sourceObjectName": "User",   "targetObjectName": "User"`).
    - Fügen Sie in der **ObjectMapping** [AttributeMappings](synchronization-attributemapping.md) Zeichenfolgenarray einen neuen Eintrag hinzu, wie im folgenden Beispiel dargestellt.

```json
{  
    "directories": [
    {
        "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
            "name": "salesforce.com",
            "objects": [
            {
                "attributes": [
                        {
                            "name": "officeCode",
                            "type": "String"
                        }
                ],
                "name":"User"
            }]
    }
    ],
    "synchronizationRules": [
        {
        "editable": true,
        "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
        "name": "USER_OUTBOUND_USER",
        "objectMappings": [
            {
            "attributeMappings": [
                {
                    "source": {
                            "name": "extensionAttribute10",
                            "type": "Attribute"
                        },
                    "targetAttributeName": "officeCode"
                }
            ],
            "name": "Synchronize Azure Active Directory Users to salesforce.com",
            "scope": null,
            "sourceObjectName": "User",
            "targetObjectName": "User"
            }
        ],
    "priority": 1,
        "sourceDirectoryName": "Azure Active Directory",
        "targetDirectoryName": "salesforce.com"
    }
    ]
}
```

## <a name="save-the-modified-synchronization-schema"></a>Speichern Sie das geänderte Synchronisierungsschema

Wenn Sie das Synchronisierungsschema der aktualisierten speichern, stellen Sie sicher, dass Sie das gesamte Schema, einschließlich der unveränderten Teile enthalten. Diese Anforderung wird das vorhandene Schema durch das Objekt ersetzen, die Sie bereitstellen.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

Wenn das Schema erfolgreich gespeichert wurde, auf die nächste Iteration des Synchronisierungsauftrags, wird es mit der Verarbeitung erneut alle Konten in Ihrer Azure AD, und die neuen Zuordnungen für alle bereitgestellten Konten angewendet werden.
