---
title: Vorlage für Gruppeneinstellung abrufen
description: Eine Vorlage für Gruppeneinstellungen ist eine Vorlage mit Einstellungen, aus denen Einstellungen innerhalb eines Mandanten erstellt werden können. Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des groupSettingTemplate-Objekts, einschließlich der verfügbaren Einstellungen und ihrer Standardwerte.
localization_priority: Normal
ms.openlocfilehash: 17e385c564337fcaa1255685e2b5808caec5cba4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804998"
---
# <a name="get-a-group-setting-template"></a><span data-ttu-id="9a83a-104">Vorlage für Gruppeneinstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="9a83a-104">Get a group setting template</span></span>

<span data-ttu-id="9a83a-p102">Eine Vorlage für Gruppeneinstellungen ist eine Vorlage mit Einstellungen, aus denen Einstellungen innerhalb eines Mandanten erstellt werden können. Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekts, einschließlich der verfügbaren Einstellungen und ihrer Standardwerte.</span><span class="sxs-lookup"><span data-stu-id="9a83a-p102">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a83a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a83a-107">Permissions</span></span>

<span data-ttu-id="9a83a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a83a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a83a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a83a-110">Permission type</span></span>      | <span data-ttu-id="9a83a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a83a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a83a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a83a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a83a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a83a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a83a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a83a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a83a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a83a-115">Not supported.</span></span>    |
|<span data-ttu-id="9a83a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a83a-116">Application</span></span> | <span data-ttu-id="9a83a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a83a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a83a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a83a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a83a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9a83a-119">Optional query parameters</span></span>
<span data-ttu-id="9a83a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9a83a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a83a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a83a-121">Request headers</span></span>
| <span data-ttu-id="9a83a-122">Name</span><span class="sxs-lookup"><span data-stu-id="9a83a-122">Name</span></span> | <span data-ttu-id="9a83a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9a83a-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9a83a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a83a-124">Authorization</span></span> | <span data-ttu-id="9a83a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a83a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a83a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a83a-127">Request body</span></span>
<span data-ttu-id="9a83a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a83a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a83a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a83a-129">Response</span></span>

<span data-ttu-id="9a83a-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a83a-130">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a83a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a83a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a83a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a83a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="9a83a-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a83a-133">Response</span></span>

<span data-ttu-id="9a83a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a83a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
