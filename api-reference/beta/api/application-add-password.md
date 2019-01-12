---
title: Anwendung Kennwort hinzufügen
description: Fügt ein sicheres Kennwort zu einer Anwendung.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 565fbab9ff2cde34bcccbe760692df9d3c0d1a14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966762"
---
# <a name="add-application-password"></a><span data-ttu-id="13967-103">Anwendung Kennwort hinzufügen</span><span class="sxs-lookup"><span data-stu-id="13967-103">Add application password</span></span>

> <span data-ttu-id="13967-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13967-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13967-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13967-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13967-106">Fügt ein sicheres Kennwort zu einer Anwendung.</span><span class="sxs-lookup"><span data-stu-id="13967-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="13967-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13967-107">Permissions</span></span>
<span data-ttu-id="13967-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13967-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13967-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13967-110">Permission type</span></span>      | <span data-ttu-id="13967-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13967-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13967-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13967-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13967-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="13967-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="13967-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13967-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13967-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13967-115">Not supported.</span></span>    |
|<span data-ttu-id="13967-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13967-116">Application</span></span> | <span data-ttu-id="13967-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="13967-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13967-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13967-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="13967-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13967-119">Request headers</span></span>
| <span data-ttu-id="13967-120">Name</span><span class="sxs-lookup"><span data-stu-id="13967-120">Name</span></span>       | <span data-ttu-id="13967-121">Typ</span><span class="sxs-lookup"><span data-stu-id="13967-121">Type</span></span> | <span data-ttu-id="13967-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13967-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13967-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13967-123">Authorization</span></span>  | <span data-ttu-id="13967-124">string</span><span class="sxs-lookup"><span data-stu-id="13967-124">string</span></span>  | <span data-ttu-id="13967-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13967-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13967-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13967-127">Request body</span></span>
<span data-ttu-id="13967-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13967-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13967-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="13967-129">Response</span></span>

<span data-ttu-id="13967-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und das Kennwort im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="13967-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="13967-131">Azure AD generiert ein sicheres Kennwort, der zurückgegeben wird, über die `secretText` Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="13967-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="13967-132">Es ist nicht möglich, das Kennwort in der Zukunft abrufen.</span><span class="sxs-lookup"><span data-stu-id="13967-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="13967-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13967-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13967-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13967-134">Request</span></span>
<span data-ttu-id="13967-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13967-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="13967-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="13967-136">Response</span></span>
<span data-ttu-id="13967-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="13967-137">Here is an example of the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "customKeyIdentifier": "Binary",
    "endDateTime": "String (timestamp)",
    "keyId": "String (identifier)",
    "startDateTime": "String (timestamp)",
    "secretText": "String",
    "hint": "String"
}
```
