---
title: Konfigurieren der Synchronisierung mit Verzeichnis Extension-Attribute
description: 'Sie können das Synchronisierungsschema zum Einschließen von Azure Active Directory (AD Azure) Erweiterung Verzeichnisattributen anpassen. In diesem Artikel wird beschrieben, wie mithilfe einer Directory Extension-Attribut (**extension_9d98asdfl15980a_Nickname**) den Wert des User.CommunityNickname in Vertriebs aufgefüllt wird. In diesem Szenario müssen Sie Azure AD-Connect richten Sie eine Reihe von Attributen Erweiterung Directory von Windows Server Active Directory lokalen Azure AD bereit. '
localization_priority: Normal
ms.openlocfilehash: 4160a95acfc6b23f5d5a9d880f36d9ca6a1f3362
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523862"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>Konfigurieren der Synchronisierung mit Verzeichnis Extension-Attribute

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können das Synchronisierungsschema zum Einschließen von Azure Active Directory (AD Azure) Erweiterung Verzeichnisattributen anpassen. In diesem Artikel wird beschrieben, wie mithilfe einer Directory Extension-Attribut (**extension_9d98asdfl15980a_Nickname**) den Wert des User.CommunityNickname in Vertriebs aufgefüllt wird. In diesem Szenario müssen Sie Azure AD-Connect richten Sie eine Reihe von Attributen Erweiterung Directory von Windows Server Active Directory lokalen Azure AD bereit. 

In diesem Artikel wird davon ausgegangen, dass Sie bereits eine Anwendung hinzugefügt haben, die von der Synchronisierung Ihres Mandanten über das [Portal Azure](https://portal.azure.com)unterstützt, dass Sie den Anzeigenamen der Anwendung kennen und Sie Authentifizierungstoken für Microsoft Graph verfügen. Informationen dazu, wie Sie das Autorisierungstoken erhalten möchten finden Sie unter [Get-Zugriff zum Aufrufen von Microsoft Graph-Token](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="find-the-service-principal-object-by-display-name"></a>Hier finden Sie das principal-Objekt nach Anzeigename

Im folgenden Beispiel wird veranschaulicht, wie ein Service principal-Objekt mit dem Anzeigenamen "Vertriebs Sandkasten" suchen.

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}
```

```json
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

Die `{servicePrincipalId}` ist `60443998-8cf7-4e61-b05c-a53b658cb5e1`.

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>Synchronisierungsaufträge im Zusammenhang mit den Dienstprinzipal auflisten 

Das folgende Beispiel veranschaulicht das Abrufen der `jobId` , die Sie benötigen entwickelt. Im Allgemeinen gibt die Antwort nur einen Auftrag zurück.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}
```

```json
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

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>Suchen Sie den Namen des gewünschten Verzeichnis Extension-Attributs

Sie benötigen den vollständigen Namen des Attributs Erweiterung. Wenn Sie den vollständigen Namen nicht kennen (die **extension_9d98asdfl15980a_Nickname**ähnlich aussehen sollte), finden Sie die folgende Informationen zur Erweiterung von Verzeichnisattributen und wie Sie darauf überprüfen: 

* [Erweitern des Azure AD-Directory-Schemas mit benutzerdefinierten Eigenschaften](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [Directory-Erweiterungen | Diagramm-API-Konzepte](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>Fügen Sie eine Definition für das Verzeichnis Extension-Attribut und eine Zuordnung zwischen den Attributen

Verwenden Sie, um eine nur-Text-Editor Ihrer Wahl (beispielsweise [Editor ++](https://notepad-plus-plus.org/) oder [JSON Editor Online](https://www.jsoneditoronline.org/)):

1. Hinzufügen einer [Attributdefinition](synchronization-attributedefinition.md) für die `extension_9d98asdfl15980a_Nickname` Attribut. 

    - Klicken Sie unter Verzeichnisse Hier finden Sie das Verzeichnis mit dem Namen "Azure Active Directory", und suchen Sie in der Objekt-Array, der eine benannte **Benutzer**.
    - Fügen Sie das neue Attribut zur Liste der Name und Typ, angeben, wie im folgenden Beispiel dargestellt.

2. Fügen Sie ein [Attribut Zuordnung](synchronization-attributemapping.md) zwischen extension_9d98asdfl15980a_Nickname und CommunityNickname hinzu.

    - Unter [SynchronizationRules](synchronization-synchronizationrule.md), suchen Sie die Regel, die Azure AD als Quellverzeichnis und Salesforce.com als das Zielverzeichnis angibt (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).
    - Suchen Sie in der [ObjectMappings](synchronization-objectmapping.md) der Regel, die Zuordnung zwischen Benutzern (`"sourceObjectName": "User",   "targetObjectName": "User"`).
    - Fügen Sie in der **ObjectMapping** [AttributeMappings](synchronization-attributemapping.md) Zeichenfolgenarray einen neuen Eintrag hinzu, wie im folgenden Beispiel dargestellt.

    ```json
    {
        "directories": [
            {
                "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
                "name": "Azure Active Directory",
                "objects": [
                    {
                        "attributes": [
                                ,{
                                "name": "extension_9d98asdfl15980a_Nickname",
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
            "metadata": [..],
            "name": "USER_OUTBOUND_USER",
            "objectMappings": [
                {
                    "attributeMappings": [
                    ,{
                        "source": {
                            "name": "extension_9d98asdfl15980a_Nickname",
                            "type": "Attribute"
                        },
                        "targetAttributeName": "CommunityNickname"
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
            },
        ]
    }
    ```

## <a name="save-the-modified-synchronization-schema"></a>Speichern Sie das geänderte Synchronisierungsschema

Wenn Sie das Synchronisierungsschema der aktualisierten speichern, stellen Sie sicher, dass Sie das gesamte Schema, einschließlich der unveränderten Teile enthalten. Diese Anforderung wird das vorhandene Schema durch das Objekt ersetzen, die Sie bereitstellen.

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

Wenn das Schema erfolgreich gespeichert wurde, auf die nächste Iteration des Synchronisierungsauftrags, wird es mit der Verarbeitung erneut alle Konten in Ihrer Azure AD, und die neuen Zuordnungen für alle bereitgestellten Konten angewendet werden.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-directory-extension-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
