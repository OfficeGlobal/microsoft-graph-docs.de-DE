---
title: List groupSettingTemplates
description: Gruppeneinstellungsvorlagen stellen einen Satz von Vorlagen dar, aus dem Gruppeneinstellungen erstellt und in einem Mandanten verwendet werden können.  Dieser Vorgang ruft die Liste der verfügbaren groupSettingTemplates-Objekte ab.
ms.openlocfilehash: e3a92b174b4d1d95cbbf22385b56484441a6e3eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019558"
---
# <a name="list-groupsettingtemplates"></a><span data-ttu-id="c89b4-104">List groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="c89b4-104">List groupSettingTemplates</span></span>

<span data-ttu-id="c89b4-p102">Gruppeneinstellungsvorlagen stellen einen Satz von Vorlagen dar, aus dem Gruppeneinstellungen erstellt und in einem Mandanten verwendet werden können.  Dieser Vorgang ruft die Liste der verfügbaren groupSettingTemplates-Objekte ab.</span><span class="sxs-lookup"><span data-stu-id="c89b4-p102">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c89b4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c89b4-107">Permissions</span></span>

<span data-ttu-id="c89b4-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89b4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c89b4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c89b4-110">Permission type</span></span>      | <span data-ttu-id="c89b4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c89b4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c89b4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c89b4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c89b4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c89b4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c89b4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c89b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c89b4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c89b4-115">Not supported.</span></span>    |
|<span data-ttu-id="c89b4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c89b4-116">Application</span></span> | <span data-ttu-id="c89b4-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89b4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c89b4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c89b4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c89b4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c89b4-119">Optional query parameters</span></span>
<span data-ttu-id="c89b4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c89b4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="c89b4-121">**Hinweis:** $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c89b4-121">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c89b4-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c89b4-122">Request headers</span></span>
| <span data-ttu-id="c89b4-123">Name</span><span class="sxs-lookup"><span data-stu-id="c89b4-123">Name</span></span> | <span data-ttu-id="c89b4-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c89b4-124">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c89b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89b4-125">Authorization</span></span>  | <span data-ttu-id="c89b4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c89b4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c89b4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c89b4-128">Request body</span></span>
<span data-ttu-id="c89b4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c89b4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c89b4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c89b4-130">Response</span></span>

<span data-ttu-id="c89b4-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c89b4-131">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c89b4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c89b4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c89b4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c89b4-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="c89b4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c89b4-134">Response</span></span>

<span data-ttu-id="c89b4-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c89b4-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
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
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->