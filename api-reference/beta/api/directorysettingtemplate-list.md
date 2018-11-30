---
title: Liste directorySettingTemplates
description: Festlegen von Vorlagen Directory stellt einen Satz von Vorlagen für Directory-Einstellungen aus dem, die Verzeichnis Einstellungen erstellt und innerhalb einer mandantenstruktur verwendet werden können.  Dieser Vorgang wird die Liste der verfügbaren DirectorySettingTemplates Objekte abgerufen.
ms.openlocfilehash: 964e2cfc9e06b6a996f63c92cae830e03c953cd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062708"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="afd39-104">Liste directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="afd39-104">List directorySettingTemplates</span></span>

> <span data-ttu-id="afd39-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="afd39-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afd39-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afd39-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afd39-107">Festlegen von Vorlagen Directory stellt einen Satz von Vorlagen für Directory-Einstellungen aus dem, die Verzeichnis Einstellungen erstellt und innerhalb einer mandantenstruktur verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="afd39-107">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="afd39-108">Dieser Vorgang wird die Liste der verfügbaren DirectorySettingTemplates Objekte abgerufen.</span><span class="sxs-lookup"><span data-stu-id="afd39-108">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="afd39-109">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="afd39-109">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="afd39-110">Die Version /v1.0 dieser API wurde in der *Liste GroupSettingTemplate*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="afd39-110">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd39-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="afd39-111">Permissions</span></span>
<span data-ttu-id="afd39-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd39-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afd39-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afd39-114">Permission type</span></span>      | <span data-ttu-id="afd39-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afd39-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afd39-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afd39-116">Delegated (work or school account)</span></span> | <span data-ttu-id="afd39-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afd39-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="afd39-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afd39-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afd39-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="afd39-119">Not supported.</span></span>    |
|<span data-ttu-id="afd39-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afd39-120">Application</span></span> | <span data-ttu-id="afd39-121">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afd39-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afd39-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afd39-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afd39-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="afd39-123">Optional query parameters</span></span>
<span data-ttu-id="afd39-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="afd39-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd39-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afd39-125">Request headers</span></span>
| <span data-ttu-id="afd39-126">Name</span><span class="sxs-lookup"><span data-stu-id="afd39-126">Name</span></span>      |<span data-ttu-id="afd39-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afd39-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="afd39-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="afd39-128">Authorization</span></span>  | <span data-ttu-id="afd39-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="afd39-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afd39-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afd39-131">Request body</span></span>
<span data-ttu-id="afd39-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="afd39-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd39-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="afd39-133">Response</span></span>

<span data-ttu-id="afd39-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DirectorySettingTemplate](../resources/directorysettingtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="afd39-134">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afd39-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afd39-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afd39-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afd39-136">Request</span></span>
<span data-ttu-id="afd39-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afd39-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="afd39-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="afd39-138">Response</span></span>
<span data-ttu-id="afd39-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afd39-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->