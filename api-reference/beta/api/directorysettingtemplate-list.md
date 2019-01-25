---
title: Liste directorySettingTemplates
description: Festlegen von Vorlagen Directory stellt einen Satz von Vorlagen für Directory-Einstellungen aus dem, die Verzeichnis Einstellungen erstellt und innerhalb einer mandantenstruktur verwendet werden können.  Dieser Vorgang wird die Liste der verfügbaren DirectorySettingTemplates Objekte abgerufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cd0112bd0d9f98f969832427d497d6e9ba2aa14
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530104"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="82374-104">Liste directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="82374-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82374-105">Festlegen von Vorlagen Directory stellt einen Satz von Vorlagen für Directory-Einstellungen aus dem, die Verzeichnis Einstellungen erstellt und innerhalb einer mandantenstruktur verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="82374-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="82374-106">Dieser Vorgang wird die Liste der verfügbaren DirectorySettingTemplates Objekte abgerufen.</span><span class="sxs-lookup"><span data-stu-id="82374-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="82374-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="82374-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="82374-108">Die Version /v1.0 dieser API wurde in der *Liste GroupSettingTemplate*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="82374-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="82374-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="82374-109">Permissions</span></span>
<span data-ttu-id="82374-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82374-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82374-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="82374-112">Permission type</span></span>      | <span data-ttu-id="82374-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="82374-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82374-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="82374-114">Delegated (work or school account)</span></span> | <span data-ttu-id="82374-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82374-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82374-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="82374-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82374-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="82374-117">Not supported.</span></span>    |
|<span data-ttu-id="82374-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="82374-118">Application</span></span> | <span data-ttu-id="82374-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82374-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82374-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="82374-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82374-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="82374-121">Optional query parameters</span></span>
<span data-ttu-id="82374-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="82374-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82374-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="82374-123">Request headers</span></span>
| <span data-ttu-id="82374-124">Name</span><span class="sxs-lookup"><span data-stu-id="82374-124">Name</span></span>      |<span data-ttu-id="82374-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82374-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82374-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="82374-126">Authorization</span></span>  | <span data-ttu-id="82374-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="82374-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82374-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="82374-129">Request body</span></span>
<span data-ttu-id="82374-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="82374-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82374-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="82374-131">Response</span></span>

<span data-ttu-id="82374-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DirectorySettingTemplate](../resources/directorysettingtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="82374-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82374-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="82374-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82374-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="82374-134">Request</span></span>
<span data-ttu-id="82374-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="82374-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="82374-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="82374-136">Response</span></span>
<span data-ttu-id="82374-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82374-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "description": "description-value",
      "values": [
        {
          "name": "name-value",
          "type": "type-value",
          "defaultValue": "defaultValue-value",
          "description": "description-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
