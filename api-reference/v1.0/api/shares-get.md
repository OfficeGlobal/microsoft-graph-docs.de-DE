---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Zugriff auf freigegebene Elemente
localization_priority: Normal
ms.openlocfilehash: fbde377c05b4b1f86bff32afcbaf0023c9be487a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831528"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="cde62-102">Zugriff auf freigegebene DriveItems</span><span class="sxs-lookup"><span data-stu-id="cde62-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="cde62-103">Verwenden Sie für den Zugriff auf ein freigegebenes [DriveItem](../resources/driveitem.md)-Element oder eine Sammlung freigegebener Elemente eine **shareId** oder Freigabe-URL.</span><span class="sxs-lookup"><span data-stu-id="cde62-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="cde62-104">Um eine Freigabe-URL mit dieser API verwenden zu können, muss die App [die URL in ein Freigabetoken konvertieren](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="cde62-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="cde62-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cde62-105">Permissions</span></span>

<span data-ttu-id="cde62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cde62-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cde62-108">Permission type</span></span>      | <span data-ttu-id="cde62-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cde62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cde62-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cde62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cde62-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde62-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cde62-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cde62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde62-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde62-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cde62-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cde62-114">Application</span></span> | <span data-ttu-id="cde62-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cde62-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cde62-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cde62-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="cde62-117">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="cde62-117">Path Parameters</span></span>

| <span data-ttu-id="cde62-118">Parametername</span><span class="sxs-lookup"><span data-stu-id="cde62-118">Parameter Name</span></span>        | <span data-ttu-id="cde62-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cde62-119">Value</span></span>    | <span data-ttu-id="cde62-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cde62-120">Description</span></span>                                                                         |
|:----------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="cde62-121">**sharingTokenOrUrl**</span><span class="sxs-lookup"><span data-stu-id="cde62-121">**sharingTokenOrUrl**</span></span> | `string` | <span data-ttu-id="cde62-122">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cde62-122">Required.</span></span> <span data-ttu-id="cde62-123">Ein Freigabetoken, wie es von der API oder einer ordnungsgemäß codierten Freigabe-URL zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="cde62-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="cde62-124">Codieren von Freigabe-URLs</span><span class="sxs-lookup"><span data-stu-id="cde62-124">Encoding sharing URLs</span></span>

<span data-ttu-id="cde62-125">Verwenden Sie zum Codieren einer Freigabe-URL die folgende Logik:</span><span class="sxs-lookup"><span data-stu-id="cde62-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="cde62-126">Als Erstes codieren Sie die URL mithilfe von Base64.</span><span class="sxs-lookup"><span data-stu-id="cde62-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="cde62-127">Konvertieren Sie das Base64-codierte Ergebnis in das [base64url-Format ohne Füllzeichen](https://en.wikipedia.org/wiki/Base64), indem Sie `=`-Zeichen vom Ende des Werts entfernen und `/` durch `_` sowie `+` durch `-` ersetzen.</span><span class="sxs-lookup"><span data-stu-id="cde62-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="cde62-128">Fügen Sie `u!` an den Anfang der Zeichenfolge an.</span><span class="sxs-lookup"><span data-stu-id="cde62-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="cde62-129">Beispiel für die Codierung einer URL in C#:</span><span class="sxs-lookup"><span data-stu-id="cde62-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="response"></a><span data-ttu-id="cde62-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="cde62-130">Response</span></span>

<span data-ttu-id="cde62-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [sharedDriveItem](../resources/shareddriveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cde62-131">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cde62-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cde62-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cde62-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cde62-133">Request</span></span>

<span data-ttu-id="cde62-134">Im Folgenden finden Sie ein Beispiel für die Anforderung zum Abrufen eines freigegebenen Elements:</span><span class="sxs-lookup"><span data-stu-id="cde62-134">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="cde62-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cde62-135">Response</span></span>

<span data-ttu-id="cde62-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cde62-136">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="cde62-137">Direkter Zugriff auf das freigegebene Element</span><span class="sxs-lookup"><span data-stu-id="cde62-137">Access the shared item directly</span></span>

<span data-ttu-id="cde62-p103">Obwohl das [**SharedDriveItem**](../resources/shareddriveitem.md)-Element nützliche Informationen enthält, möchten die meisten Apps direkt auf das freigegebene [DriveItem](../resources/driveitem.md)-Element zugreifen. Die **SharedDriveItem**-Ressource umfasst **root**- und **items**-Beziehungen, die innerhalb des Bereichs des freigegebenen Elements auf die Inhalte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="cde62-p103">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="cde62-140">Beispiel (einzelne Datei)</span><span class="sxs-lookup"><span data-stu-id="cde62-140">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="cde62-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cde62-141">Request</span></span>

<span data-ttu-id="cde62-142">Durch das Anfordern der **driveItem**-Beziehung wird das **DriveItem**-Element zurückgegeben, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="cde62-142">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="cde62-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="cde62-143">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="cde62-144">Beispiel (freigegebener Ordner)</span><span class="sxs-lookup"><span data-stu-id="cde62-144">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="cde62-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cde62-145">Request</span></span>

<span data-ttu-id="cde62-146">Durch das Anfordern der **driveItem**-Beziehung und das Erweitern der **children**-Sammlung wird das freigegebene **DriveItem**-Element mit Dateien im freigegebenen Ordner zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cde62-146">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="cde62-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="cde62-147">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="error-responses"></a><span data-ttu-id="cde62-148">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="cde62-148">Error Responses</span></span>

<span data-ttu-id="cde62-149">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="cde62-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="cde62-150">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="cde62-150">Remarks</span></span>

* <span data-ttu-id="cde62-151">Bei OneDrive for Business und SharePoint erfordert die Freigabe-API immer eine Authentifizierung und kann nicht verwendet werden, um auf anonym freigegebene Inhalte ohne Benutzerkontext zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="cde62-151">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
