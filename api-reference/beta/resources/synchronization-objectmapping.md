---
title: Ressourcentyp objectMapping
description: Definiert, wie ein bestimmtes Objekt aus dem Quellverzeichnis zum Zielverzeichnis synchronisiert werden sollen. Insbesondere wird definiert, wie-Objekts in Quellverzeichnis ein Objekt im Zielverzeichnis, zugeordnet werden soll was (falls vorhanden) festlegen des Gültigkeitsbereichs Filter sollte verwendet werden, zu entscheiden, ob wir ein bestimmtes Objekt bereitstellen möchten, und Wechsel zu von transformiert wie Objektattribute werden sollten Quell-und Zielverzeichnis.
localization_priority: Normal
ms.openlocfilehash: 274d401c28abc25d904c259b00a673f3c0a53888
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526914"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="4b770-104">Ressourcentyp objectMapping</span><span class="sxs-lookup"><span data-stu-id="4b770-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b770-105">Definiert, wie ein bestimmtes Objekt aus dem Quellverzeichnis zum Zielverzeichnis synchronisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="4b770-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="4b770-106">Insbesondere wird definiert, wie-Objekts in Quellverzeichnis ein Objekt im Zielverzeichnis, zugeordnet werden soll was (falls vorhanden) festlegen des Gültigkeitsbereichs Filter sollte verwendet werden, zu entscheiden, ob wir ein bestimmtes Objekt bereitstellen möchten, und Wechsel zu von transformiert wie Objektattribute werden sollten Quell-und Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4b770-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="4b770-107">Objekt Zuordnungen der Hauptteil der [Synchronisierung Regel](synchronization-synchronizationrule.md) werden und werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4b770-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b770-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b770-108">Properties</span></span>

| <span data-ttu-id="4b770-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b770-109">Property</span></span>      | <span data-ttu-id="4b770-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4b770-110">Type</span></span>      | <span data-ttu-id="4b770-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b770-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4b770-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="4b770-112">attributeMappings</span></span>  |<span data-ttu-id="4b770-113">[AttributeMapping](synchronization-attributemapping.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4b770-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="4b770-114">Attribut Zuordnungen definieren, welche Attribute zuordnen aus dem Quellobjekt in das Zielobjekt und wie übertragen werden soll.</span><span class="sxs-lookup"><span data-stu-id="4b770-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="4b770-115">Eine Reihe von Funktionen stehen die Transformation der ursprünglichen Quellwerte unterstützen.</span><span class="sxs-lookup"><span data-stu-id="4b770-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="4b770-116">enabled</span><span class="sxs-lookup"><span data-stu-id="4b770-116">enabled</span></span>        |<span data-ttu-id="4b770-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b770-117">Boolean</span></span>    |<span data-ttu-id="4b770-118">Wenn `true`, diese objektzuordnung während der Synchronisation verarbeitet werden.</span><span class="sxs-lookup"><span data-stu-id="4b770-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="4b770-119">Wenn `false`, diese objektzuordnung übersprungen.</span><span class="sxs-lookup"><span data-stu-id="4b770-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="4b770-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="4b770-120">flowTypes</span></span>      |<span data-ttu-id="4b770-121">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="4b770-121">objectFlowType</span></span>    |<span data-ttu-id="4b770-122">Welche Ablauf für diese objektzuordnung aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="4b770-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="4b770-123">`Add`erstellt neue Objekte in das Zielverzeichnis `Update` ändert vorhandene Objekte und `Delete` Verwaltungsagents vorhandener Benutzer.</span><span class="sxs-lookup"><span data-stu-id="4b770-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="4b770-124">Der Standardwert ist `Add, Update, Delete`.</span><span class="sxs-lookup"><span data-stu-id="4b770-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="4b770-125">$metadata</span><span class="sxs-lookup"><span data-stu-id="4b770-125">metadata</span></span>       |<span data-ttu-id="4b770-126">MetadataEntry-Auflistung</span><span class="sxs-lookup"><span data-stu-id="4b770-126">metadataEntry collection</span></span>    |<span data-ttu-id="4b770-127">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4b770-127">Additional extension properties.</span></span> <span data-ttu-id="4b770-128">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="4b770-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4b770-129">name</span><span class="sxs-lookup"><span data-stu-id="4b770-129">name</span></span>           |<span data-ttu-id="4b770-130">String</span><span class="sxs-lookup"><span data-stu-id="4b770-130">String</span></span>     |<span data-ttu-id="4b770-131">Human-Anzeigenamen des Objekt-Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="4b770-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="4b770-132">Bereich</span><span class="sxs-lookup"><span data-stu-id="4b770-132">scope</span></span>          |[<span data-ttu-id="4b770-133">filter</span><span class="sxs-lookup"><span data-stu-id="4b770-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="4b770-134">Definiert einen Filter verwendet werden, bei der Entscheidung, ob ein bestimmtes Objekt bereitgestellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="4b770-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="4b770-135">Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden.</span><span class="sxs-lookup"><span data-stu-id="4b770-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="4b770-136">Objektname (Herkunft)</span><span class="sxs-lookup"><span data-stu-id="4b770-136">sourceObjectName</span></span>           |<span data-ttu-id="4b770-137">String</span><span class="sxs-lookup"><span data-stu-id="4b770-137">String</span></span>     |<span data-ttu-id="4b770-138">Name des Objekts in das Quellverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4b770-138">Name of the object in the source directory.</span></span> <span data-ttu-id="4b770-139">Muss die zu verwendenden Objektnamen aus der Quelle [Directory Definition](synchronization-directorydefinition.md)übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4b770-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="4b770-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="4b770-140">targetObjectName</span></span>           |<span data-ttu-id="4b770-141">String</span><span class="sxs-lookup"><span data-stu-id="4b770-141">String</span></span>     |<span data-ttu-id="4b770-142">Name des Objekts in das Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="4b770-142">Name of the object in target directory.</span></span> <span data-ttu-id="4b770-143">Muss die zu verwendenden Objektnamen aus der Ziel- [Verzeichnis Definition](synchronization-directorydefinition.md)übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="4b770-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b770-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b770-144">JSON representation</span></span>

<span data-ttu-id="4b770-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b770-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="4b770-146">Beispiel von JSON</span><span class="sxs-lookup"><span data-stu-id="4b770-146">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
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
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Mid([userPrincipalName], 1, 8)",
                "name": "Mid",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[userPrincipalName]",
                            "name": "userPrincipalName",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "start",
                        "value": {
                            "expression": "\"1\"",
                            "name": "1",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "length",
                        "value": {
                            "expression": "\"8\"",
                            "name": "8",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "Alias"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[mail]",
                "name": "mail",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Email"
        },
        {
            "defaultValue": "ISO-8859-1",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "EmailEncodingKey"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "LanguageLocaleKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[givenName]",
                "name": "givenName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "FirstName"
        },
        {
            "defaultValue": ".",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[surname]",
                "name": "surname",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "LastName"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
                "name": "Replace",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[preferredLanguage]",
                            "name": "preferredLanguage",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "Find",
                        "value": {
                            "expression": "\"-\"",
                            "name": "-",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "Replacement",
                        "value": {
                            "expression": "\"_\"",
                            "name": "_",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "LocaleSidKey"
        },
        {
            "defaultValue": "Chatter Free User",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "SingleAppRoleAssignment([appRoleAssignments])",
                "name": "SingleAppRoleAssignment",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[appRoleAssignments]",
                            "name": "appRoleAssignments",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "ProfileName"
        },
        {
            "defaultValue": "America/Los_Angeles",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "TimeZoneSidKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 1,
            "source": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Username"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsCallCenterAutoLogin"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsMarketingUser"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsOfflineUser"
        }
    ],
    "enabled": true,
    "flowTypes": "Add, Update, Delete",
    "metadata": [
        {
            "key": "IsCustomerDefined",
            "value": "false"
        },
        {
            "key": "DisableMonitoringForChanges",
            "value": "false"
        },
        {
            "key": "Disposition",
            "value": "\"Normal\""
        },
        {
            "key": "ExcludeFromReporting",
            "value": "false"
        },
        {
            "key": "EscrowBehavior",
            "value": "\"Default\""
        },
        {
            "key": "Unsynchronized",
            "value": "false"
        }
    ],
    "name": "Synchronize Azure Active Directory Users to salesforce.com",
    "scope": null,
    "sourceObjectName": "User",
    "targetObjectName": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectmapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
