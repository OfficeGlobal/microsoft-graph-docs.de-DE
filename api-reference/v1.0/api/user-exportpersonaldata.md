---
title: 'Benutzer: ExportPersonalData'
description: Fordert die Daten Richtlinie Vorgang, versucht ein Unternehmensadministrator, eine Organisationseinheit Benutzerdaten exportieren.
ms.openlocfilehash: 7d41d6d855fee992a4ff3a542e6c11f692adcfe3
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284133"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="f7e07-103">Benutzer: ExportPersonalData</span><span class="sxs-lookup"><span data-stu-id="f7e07-103">user: exportPersonalData</span></span>

<span data-ttu-id="f7e07-104">Fordern Sie ein Daten Richtlinie Vorgang aus ein Unternehmensadministrator oder einer Anwendung zum Exportieren von Daten für eine Organisationseinheit des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f7e07-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e07-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7e07-105">Permissions</span></span>
<span data-ttu-id="f7e07-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e07-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f7e07-108">Permission type</span></span>      | <span data-ttu-id="f7e07-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f7e07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e07-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f7e07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7e07-111">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e07-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="f7e07-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f7e07-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7e07-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="f7e07-113">Not applicable</span></span>  |
|<span data-ttu-id="f7e07-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f7e07-114">Application</span></span> | <span data-ttu-id="f7e07-115">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e07-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="f7e07-116">**Hinweis:** Der Exportvorgang kann nur von einem Unternehmensadministrator ausgeführt werden, wenn delegierte Berechtigungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f7e07-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7e07-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7e07-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="f7e07-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f7e07-118">Request headers</span></span>
| <span data-ttu-id="f7e07-119">Name</span><span class="sxs-lookup"><span data-stu-id="f7e07-119">Name</span></span>       | <span data-ttu-id="f7e07-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7e07-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7e07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e07-121">Authorization</span></span>  | <span data-ttu-id="f7e07-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f7e07-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e07-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f7e07-123">Request body</span></span>
<span data-ttu-id="f7e07-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="f7e07-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7e07-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="f7e07-125">Parameter</span></span>    | <span data-ttu-id="f7e07-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f7e07-126">Type</span></span>   |<span data-ttu-id="f7e07-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7e07-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7e07-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="f7e07-128">storageLocation</span></span>|<span data-ttu-id="f7e07-129">String</span><span class="sxs-lookup"><span data-stu-id="f7e07-129">String</span></span>|<span data-ttu-id="f7e07-130">Dies ist die URL einer gemeinsamen Zugriff Signatur (SAS) ein Konto Azure-Speicher an, in dem Daten exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f7e07-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="f7e07-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7e07-131">Response</span></span>
<span data-ttu-id="f7e07-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202 Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7e07-p102">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e07-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7e07-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7e07-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7e07-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="f7e07-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7e07-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
