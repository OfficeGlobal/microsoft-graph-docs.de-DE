---
title: Ressourcentyp userSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517239"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="372c3-104">Ressourcentyp userSecurityState</span><span class="sxs-lookup"><span data-stu-id="372c3-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="372c3-105">Statusinformationen über das Benutzerkonto enthält.</span><span class="sxs-lookup"><span data-stu-id="372c3-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="372c3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="372c3-106">Properties</span></span>

| <span data-ttu-id="372c3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="372c3-107">Property</span></span>   | <span data-ttu-id="372c3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="372c3-108">Type</span></span> |<span data-ttu-id="372c3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="372c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="372c3-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="372c3-110">aadUserId</span></span>|<span data-ttu-id="372c3-111">String</span><span class="sxs-lookup"><span data-stu-id="372c3-111">String</span></span>|<span data-ttu-id="372c3-112">AAD Benutzer Objekt-ID (GUID) - die physische/multi-account Benutzerentität darstellt.</span><span class="sxs-lookup"><span data-stu-id="372c3-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="372c3-113">accountName</span><span class="sxs-lookup"><span data-stu-id="372c3-113">accountName</span></span>|<span data-ttu-id="372c3-114">String</span><span class="sxs-lookup"><span data-stu-id="372c3-114">String</span></span>|<span data-ttu-id="372c3-115">Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch als bezeichnet `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="372c3-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="372c3-116">Domänname</span><span class="sxs-lookup"><span data-stu-id="372c3-116">domainName</span></span>|<span data-ttu-id="372c3-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="372c3-117">String</span></span>|<span data-ttu-id="372c3-118">NetBIOS/Active Directory-Domäne des Benutzerkontos (d. h., im Format Domäne\Konto).</span><span class="sxs-lookup"><span data-stu-id="372c3-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="372c3-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="372c3-119">emailRole</span></span>|<span data-ttu-id="372c3-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="372c3-120">emailRole</span></span>|<span data-ttu-id="372c3-121">Für e-Mail-bezogene Alerts - des Benutzerkontos e-Mail 'Role'.</span><span class="sxs-lookup"><span data-stu-id="372c3-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="372c3-122">Mögliche Werte sind: `unknown`, `sender` und `recipient`.</span><span class="sxs-lookup"><span data-stu-id="372c3-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="372c3-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="372c3-123">isVpn</span></span>|<span data-ttu-id="372c3-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="372c3-124">Boolean</span></span>|<span data-ttu-id="372c3-125">Gibt an, ob der Benutzer über ein VPN angemeldet.</span><span class="sxs-lookup"><span data-stu-id="372c3-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="372c3-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="372c3-126">logonDateTime</span></span>|<span data-ttu-id="372c3-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="372c3-127">DateTimeOffset</span></span>|<span data-ttu-id="372c3-128">Zeitpunkt der Anmeldung bei der aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="372c3-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="372c3-129">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="372c3-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="372c3-130">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="372c3-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="372c3-131">logonId</span><span class="sxs-lookup"><span data-stu-id="372c3-131">logonId</span></span>|<span data-ttu-id="372c3-132">String</span><span class="sxs-lookup"><span data-stu-id="372c3-132">String</span></span>|<span data-ttu-id="372c3-133">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="372c3-133">User sign-in ID.</span></span>|
|<span data-ttu-id="372c3-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="372c3-134">logonIp</span></span>|<span data-ttu-id="372c3-135">String</span><span class="sxs-lookup"><span data-stu-id="372c3-135">String</span></span>|<span data-ttu-id="372c3-136">IP-Adresse, die von die Anforderung-Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="372c3-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="372c3-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="372c3-137">logonLocation</span></span>|<span data-ttu-id="372c3-138">String</span><span class="sxs-lookup"><span data-stu-id="372c3-138">String</span></span>|<span data-ttu-id="372c3-139">Speicherort (nach Zuordnung von IP-Adresse) ein Benutzer anmelden Ereignis von diesem Benutzer zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="372c3-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="372c3-140">logonType</span><span class="sxs-lookup"><span data-stu-id="372c3-140">logonType</span></span>|<span data-ttu-id="372c3-141">logonType</span><span class="sxs-lookup"><span data-stu-id="372c3-141">logonType</span></span>|<span data-ttu-id="372c3-142">-Methode des Benutzers anmelden.</span><span class="sxs-lookup"><span data-stu-id="372c3-142">Method of user sign in.</span></span> <span data-ttu-id="372c3-143">Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.</span><span class="sxs-lookup"><span data-stu-id="372c3-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="372c3-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="372c3-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="372c3-145">String</span><span class="sxs-lookup"><span data-stu-id="372c3-145">String</span></span>|<span data-ttu-id="372c3-146">Active Directory (lokal) Sicherheits-ID (SID) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="372c3-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="372c3-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="372c3-147">riskScore</span></span>|<span data-ttu-id="372c3-148">String</span><span class="sxs-lookup"><span data-stu-id="372c3-148">String</span></span>|<span data-ttu-id="372c3-149">Provider-generiert/berechnet Risiko Bewertung des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="372c3-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="372c3-150">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="372c3-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="372c3-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="372c3-151">userAccountType</span></span>|<span data-ttu-id="372c3-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="372c3-152">userAccountSecurityType</span></span>|<span data-ttu-id="372c3-153">Typ des Benutzerkontos (Gruppenmitgliedschaft) pro Windows-Definition.</span><span class="sxs-lookup"><span data-stu-id="372c3-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="372c3-154">Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.</span><span class="sxs-lookup"><span data-stu-id="372c3-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="372c3-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="372c3-155">userPrincipalName</span></span>|<span data-ttu-id="372c3-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="372c3-156">String</span></span>|<span data-ttu-id="372c3-157">Benutzer-Anmeldename - Internetformat: (Benutzerkontonamen) @(Konto DNS-Domänennamen).</span><span class="sxs-lookup"><span data-stu-id="372c3-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="372c3-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="372c3-158">JSON representation</span></span>

<span data-ttu-id="372c3-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="372c3-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
