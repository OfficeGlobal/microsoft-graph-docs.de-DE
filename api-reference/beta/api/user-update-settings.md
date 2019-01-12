---
title: Einstellungen für Updates
description: 'Aktualisieren Sie die Eigenschaften des Settings-Objekts. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8f538d298f71ad7ef537988a29bae812015566ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913226"
---
# <a name="update-settings"></a><span data-ttu-id="fdced-103">Einstellungen für Updates</span><span class="sxs-lookup"><span data-stu-id="fdced-103">Update settings</span></span>

> <span data-ttu-id="fdced-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdced-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdced-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdced-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdced-106">Aktualisieren Sie die Eigenschaften des [Settings](../resources/user-settings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fdced-106">Update the properties of the [settings](../resources/user-settings.md) object.</span></span> <span data-ttu-id="fdced-107">Benutzer in derselben Organisation können unterschiedliche Einstellungen basierend auf ihrer Präferenz oder auf den Richtlinien der Organisation verfügen.</span><span class="sxs-lookup"><span data-stu-id="fdced-107">Users in the same organization can have different settings based on their preference or on the organization policies.</span></span> <span data-ttu-id="fdced-108">Um die aktuelle Einstellungen abrufen, finden Sie in der [aktuellen benutzereinstellungen](user-get-settings.md).</span><span class="sxs-lookup"><span data-stu-id="fdced-108">To get the user current settings, see [current user settings](user-get-settings.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fdced-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fdced-109">Permissions</span></span>

<span data-ttu-id="fdced-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdced-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdced-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fdced-112">Permission type</span></span>      | <span data-ttu-id="fdced-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fdced-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdced-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fdced-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fdced-115">User.ReadWrite User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdced-115">User.ReadWrite, User.ReadWrite.All</span></span>   |
|<span data-ttu-id="fdced-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fdced-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdced-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fdced-117">Not supported.</span></span>    |
|<span data-ttu-id="fdced-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fdced-118">Application</span></span> | <span data-ttu-id="fdced-119">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdced-119">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdced-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdced-120">HTTP request</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

<span data-ttu-id="fdced-121">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="fdced-121">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="fdced-122">Weitere Informationen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdced-122">To learn more, see [Permissions](/graph/permissions-reference).</span></span> 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a><span data-ttu-id="fdced-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fdced-123">Request headers</span></span>

| <span data-ttu-id="fdced-124">Header</span><span class="sxs-lookup"><span data-stu-id="fdced-124">Header</span></span>       | <span data-ttu-id="fdced-125">Wert</span><span class="sxs-lookup"><span data-stu-id="fdced-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="fdced-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdced-126">Authorization</span></span>  | <span data-ttu-id="fdced-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fdced-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fdced-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fdced-129">Content-Type</span></span>  | <span data-ttu-id="fdced-130">application/json</span><span class="sxs-lookup"><span data-stu-id="fdced-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fdced-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fdced-131">Request body</span></span>

<span data-ttu-id="fdced-p106">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="fdced-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fdced-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdced-135">Property</span></span>     | <span data-ttu-id="fdced-136">Typ</span><span class="sxs-lookup"><span data-stu-id="fdced-136">Type</span></span>   |<span data-ttu-id="fdced-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdced-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdced-138">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="fdced-138">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="fdced-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fdced-139">Boolean</span></span>|<span data-ttu-id="fdced-140">"True" eingestellt deaktiviere Delegieren des Zugriffs auf [Trending](../resources/insights-trending.md) API und Zugriff auf Dokumente in Office eingegangen für den Benutzer zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="fdced-140">Set to true do disable delegate access to the [Trending](../resources/insights-trending.md) API and to disable access to documents in Office Delve for the user.</span></span> <span data-ttu-id="fdced-141">Einstellung auch auf True wirkt sich auf die Relevanz des Inhalts angezeigt in Office 365 – beispielsweise vorgeschlagene in SharePoint-Startseite und in der Ansicht Discover in OneDrive für Unternehmen weniger relevante Ergebnisse anzeigen.</span><span class="sxs-lookup"><span data-stu-id="fdced-141">Setting to true also affects the relevance of the content displayed in Office 365 - for example, Suggested sites in SharePoint Home and the Discover view in OneDrive for Business show less relevant results.</span></span> <span data-ttu-id="fdced-142">Diese Einstellung entspricht dem Steuerelementzustand in [Office ausführlicher behandelt](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span><span class="sxs-lookup"><span data-stu-id="fdced-142">This setting reflects the control state in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span>|

## <a name="example"></a><span data-ttu-id="fdced-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fdced-143">Example</span></span> 

##### <a name="request"></a><span data-ttu-id="fdced-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdced-144">Request</span></span>

<span data-ttu-id="fdced-145">Es folgt eine Beispiel für eine Anforderung zum Melden Sie sich einen Benutzer von Delve und seinen Beitrag auf Content Relevanz für die gesamte Organisation zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="fdced-145">Here is an example request on how to opt-out a user from Delve and disable his contribution on content relevancy for the whole organization.</span></span>

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a><span data-ttu-id="fdced-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="fdced-146">Response</span></span>

<span data-ttu-id="fdced-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fdced-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a><span data-ttu-id="fdced-150">Batchanforderung</span><span class="sxs-lookup"><span data-stu-id="fdced-150">Batch request</span></span>

<span data-ttu-id="fdced-151">Es ist auch möglich, melden Sie sich mehrere Benutzer aus Delve und Beitrags auf Content Relevanz für die gesamte Organisation über eine Batchanforderung deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="fdced-151">It's also possible to opt-out multiple users from Delve and disable their contribution on content relevancy for the whole organization through a batch request.</span></span>
<span data-ttu-id="fdced-152">Weitere Informationen finden Sie unter [JSON Batchverarbeitung](/graph/json-batching).</span><span class="sxs-lookup"><span data-stu-id="fdced-152">To learn more, see [JSON batching](/graph/json-batching).</span></span>

<span data-ttu-id="fdced-153">**Wichtig**: nur Mitglieder der Rollengruppe [Organisationsverwaltung](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) mehrere Benutzer aktualisiert werden können.</span><span class="sxs-lookup"><span data-stu-id="fdced-153">**Important**: Only members of the [Organization Management](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) role group can update multiple users.</span></span> 


