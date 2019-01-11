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
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="b8e0c-105">Konfigurieren der Synchronisierung mit benutzerdefinierten Ziel-Attribute</span><span class="sxs-lookup"><span data-stu-id="b8e0c-105">Configure synchronization with custom target attributes</span></span>

> <span data-ttu-id="b8e0c-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8e0c-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8e0c-108">Sie können das Synchronisierungsschema, um benutzerdefinierte Attribute enthalten, die in das Zielverzeichnis definiert sind, anpassen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-108">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="b8e0c-109">In diesem Artikel wird beschrieben, wie ein Abonnement Vertriebs anpassen, indem Sie ein neues Feld namens hinzufügen `officeCode`.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-109">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="b8e0c-110">Richten Sie die Synchronisierung von Azure Active Directory (AD Azure) zu Vertriebs, und für jeden Benutzer, füllen Sie die `officeCode` Feld Vertriebs mit dem Wert aus der `extensionAttribute10` in Azure AD-Feld.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-110">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="b8e0c-111">In diesem Artikel wird davon ausgegangen, dass Sie bereits eine Anwendung hinzugefügt haben, die von der Synchronisierung Ihres Mandanten über das [Portal Azure](https://portal.azure.com)unterstützt, dass Sie den Anzeigenamen der Anwendung kennen und Sie Authentifizierungstoken für Microsoft Graph verfügen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-111">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="b8e0c-112">Informationen dazu, wie Sie das Autorisierungstoken erhalten möchten finden Sie unter [Get-Zugriff zum Aufrufen von Microsoft Graph-Token](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="b8e0c-112">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="b8e0c-113">Hier finden Sie das principal-Objekt nach Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b8e0c-113">Find the service principal object by display name</span></span>

<span data-ttu-id="b8e0c-114">Im folgenden Beispiel wird veranschaulicht, wie ein Service principal-Objekt mit dem Anzeigenamen Vertriebs suchen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-114">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="b8e0c-115">Die `{servicePrincipalId}` ist `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-115">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="b8e0c-116">Synchronisierungsaufträge im Zusammenhang mit den Dienstprinzipal auflisten</span><span class="sxs-lookup"><span data-stu-id="b8e0c-116">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="b8e0c-117">Das folgende Beispiel veranschaulicht das Abrufen der `jobId` , die Sie benötigen entwickelt.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-117">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="b8e0c-118">Im Allgemeinen gibt die Antwort nur einen Auftrag zurück.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-118">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="b8e0c-119">Die `{jobId}` ist `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-119">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="b8e0c-120">Abrufen des Synchronisierungsschemas</span><span class="sxs-lookup"><span data-stu-id="b8e0c-120">Get the synchronization schema</span></span>
<span data-ttu-id="b8e0c-121">Im folgenden Beispiel wird gezeigt, wie das Synchronisierungsschema abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-121">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="b8e0c-122">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-122">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b8e0c-123">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-123">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="b8e0c-124">Fügen Sie eine Definition für das Attribut OfficeCode und eine Zuordnung zwischen Attributen</span><span class="sxs-lookup"><span data-stu-id="b8e0c-124">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="b8e0c-125">Verwenden Sie, um eine nur-Text-Editor Ihrer Wahl (beispielsweise [Editor ++](https://notepad-plus-plus.org/) oder [JSON Editor Online](https://www.jsoneditoronline.org/)):</span><span class="sxs-lookup"><span data-stu-id="b8e0c-125">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="b8e0c-126">Hinzufügen einer [Attributdefinition](synchronization-attributedefinition.md) für die `officeCode` Attribut.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-126">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="b8e0c-127">Klicken Sie unter Verzeichnisse Hier finden Sie das Verzeichnis mit dem Namen "Salesforce.com", und klicken Sie in das Objekt-Array, suchen Sie der eine benannte **Benutzer**.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-127">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="b8e0c-128">Fügen Sie das neue Attribut zur Liste der Name und Typ, angeben, wie im folgenden Beispiel dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-128">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="b8e0c-129">Hinzufügen einer [Zuordnung zwischen Attributen](synchronization-attributemapping.md) zwischen `officeCode` und `extensionAttribute10`.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-129">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="b8e0c-130">Finden Sie unter [SynchronizationRules](synchronization-synchronizationrule.md), die Regel, die als Quellverzeichnis und Salesforce.com als das Zielverzeichnis Azure AD angibt (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span><span class="sxs-lookup"><span data-stu-id="b8e0c-130">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="b8e0c-131">Suchen Sie in der [ObjectMappings](synchronization-objectmapping.md) der Regel, die Zuordnung zwischen Benutzern (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span><span class="sxs-lookup"><span data-stu-id="b8e0c-131">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="b8e0c-132">Fügen Sie in der **ObjectMapping** [AttributeMappings](synchronization-attributemapping.md) Zeichenfolgenarray einen neuen Eintrag hinzu, wie im folgenden Beispiel dargestellt.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-132">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="b8e0c-133">Speichern Sie das geänderte Synchronisierungsschema</span><span class="sxs-lookup"><span data-stu-id="b8e0c-133">Save the modified synchronization schema</span></span>

<span data-ttu-id="b8e0c-134">Wenn Sie das Synchronisierungsschema der aktualisierten speichern, stellen Sie sicher, dass Sie das gesamte Schema, einschließlich der unveränderten Teile enthalten.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-134">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="b8e0c-135">Diese Anforderung wird das vorhandene Schema durch das Objekt ersetzen, die Sie bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-135">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="b8e0c-136">Wenn das Schema erfolgreich gespeichert wurde, auf die nächste Iteration des Synchronisierungsauftrags, wird es mit der Verarbeitung erneut alle Konten in Ihrer Azure AD, und die neuen Zuordnungen für alle bereitgestellten Konten angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="b8e0c-136">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
