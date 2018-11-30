---
title: Ressourcentyp userSecurityState
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: f530ac1a657b4049c17bdcdd40f1dd5ea734f278
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061831"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="4deba-104">Ressourcentyp userSecurityState</span><span class="sxs-lookup"><span data-stu-id="4deba-104">userSecurityState resource type</span></span>

 > <span data-ttu-id="4deba-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4deba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4deba-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4deba-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4deba-107">Statusinformationen über das Benutzerkonto enthält.</span><span class="sxs-lookup"><span data-stu-id="4deba-107">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="4deba-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4deba-108">Properties</span></span>

| <span data-ttu-id="4deba-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4deba-109">Property</span></span>   | <span data-ttu-id="4deba-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4deba-110">Type</span></span> |<span data-ttu-id="4deba-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4deba-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4deba-112">aadUserId</span><span class="sxs-lookup"><span data-stu-id="4deba-112">aadUserId</span></span>|<span data-ttu-id="4deba-113">String</span><span class="sxs-lookup"><span data-stu-id="4deba-113">String</span></span>|<span data-ttu-id="4deba-114">AAD Benutzer Objekt-ID (GUID) - die physische/multi-account Benutzerentität darstellt.</span><span class="sxs-lookup"><span data-stu-id="4deba-114">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="4deba-115">accountName</span><span class="sxs-lookup"><span data-stu-id="4deba-115">accountName</span></span>|<span data-ttu-id="4deba-116">String</span><span class="sxs-lookup"><span data-stu-id="4deba-116">String</span></span>|<span data-ttu-id="4deba-117">Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch als bezeichnet `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="4deba-117">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="4deba-118">Domänname</span><span class="sxs-lookup"><span data-stu-id="4deba-118">domainName</span></span>|<span data-ttu-id="4deba-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4deba-119">String</span></span>|<span data-ttu-id="4deba-120">NetBIOS/Active Directory-Domäne des Benutzerkontos (d. h., im Format Domäne\Konto).</span><span class="sxs-lookup"><span data-stu-id="4deba-120">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="4deba-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="4deba-121">emailRole</span></span>|<span data-ttu-id="4deba-122">emailRole</span><span class="sxs-lookup"><span data-stu-id="4deba-122">emailRole</span></span>|<span data-ttu-id="4deba-123">Für e-Mail-bezogene Alerts - des Benutzerkontos e-Mail 'Role'.</span><span class="sxs-lookup"><span data-stu-id="4deba-123">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="4deba-124">Mögliche Werte sind: `unknown`, `sender` und `recipient`.</span><span class="sxs-lookup"><span data-stu-id="4deba-124">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="4deba-125">isVpn</span><span class="sxs-lookup"><span data-stu-id="4deba-125">isVpn</span></span>|<span data-ttu-id="4deba-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4deba-126">Boolean</span></span>|<span data-ttu-id="4deba-127">Gibt an, ob der Benutzer über ein VPN angemeldet.</span><span class="sxs-lookup"><span data-stu-id="4deba-127">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="4deba-128">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="4deba-128">logonDateTime</span></span>|<span data-ttu-id="4deba-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4deba-129">DateTimeOffset</span></span>|<span data-ttu-id="4deba-130">Zeitpunkt der Anmeldung bei der aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="4deba-130">Time at which the sign-in occurred.</span></span> <span data-ttu-id="4deba-131">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="4deba-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4deba-132">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4deba-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4deba-133">logonId</span><span class="sxs-lookup"><span data-stu-id="4deba-133">logonId</span></span>|<span data-ttu-id="4deba-134">String</span><span class="sxs-lookup"><span data-stu-id="4deba-134">String</span></span>|<span data-ttu-id="4deba-135">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="4deba-135">User sign-in ID.</span></span>|
|<span data-ttu-id="4deba-136">logonIp</span><span class="sxs-lookup"><span data-stu-id="4deba-136">logonIp</span></span>|<span data-ttu-id="4deba-137">String</span><span class="sxs-lookup"><span data-stu-id="4deba-137">String</span></span>|<span data-ttu-id="4deba-138">IP-Adresse, die von die Anforderung-Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="4deba-138">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="4deba-139">logonLocation</span><span class="sxs-lookup"><span data-stu-id="4deba-139">logonLocation</span></span>|<span data-ttu-id="4deba-140">String</span><span class="sxs-lookup"><span data-stu-id="4deba-140">String</span></span>|<span data-ttu-id="4deba-141">Speicherort (nach Zuordnung von IP-Adresse) ein Benutzer anmelden Ereignis von diesem Benutzer zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="4deba-141">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="4deba-142">logonType</span><span class="sxs-lookup"><span data-stu-id="4deba-142">logonType</span></span>|<span data-ttu-id="4deba-143">logonType</span><span class="sxs-lookup"><span data-stu-id="4deba-143">logonType</span></span>|<span data-ttu-id="4deba-144">-Methode des Benutzers anmelden.</span><span class="sxs-lookup"><span data-stu-id="4deba-144">Method of user sign in.</span></span> <span data-ttu-id="4deba-145">Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.</span><span class="sxs-lookup"><span data-stu-id="4deba-145">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="4deba-146">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4deba-146">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="4deba-147">String</span><span class="sxs-lookup"><span data-stu-id="4deba-147">String</span></span>|<span data-ttu-id="4deba-148">Active Directory (lokal) Sicherheits-ID (SID) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4deba-148">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="4deba-149">riskScore</span><span class="sxs-lookup"><span data-stu-id="4deba-149">riskScore</span></span>|<span data-ttu-id="4deba-150">String</span><span class="sxs-lookup"><span data-stu-id="4deba-150">String</span></span>|<span data-ttu-id="4deba-151">Provider-generiert/berechnet Risiko Bewertung des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="4deba-151">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="4deba-152">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="4deba-152">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="4deba-153">userAccountType</span><span class="sxs-lookup"><span data-stu-id="4deba-153">userAccountType</span></span>|<span data-ttu-id="4deba-154">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="4deba-154">userAccountSecurityType</span></span>|<span data-ttu-id="4deba-155">Typ des Benutzerkontos (Gruppenmitgliedschaft) pro Windows-Definition.</span><span class="sxs-lookup"><span data-stu-id="4deba-155">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="4deba-156">Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.</span><span class="sxs-lookup"><span data-stu-id="4deba-156">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="4deba-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4deba-157">userPrincipalName</span></span>|<span data-ttu-id="4deba-158">String</span><span class="sxs-lookup"><span data-stu-id="4deba-158">String</span></span>|<span data-ttu-id="4deba-159">Benutzer-Anmeldename - Internetformat: (Benutzerkontonamen) @(Konto DNS-Domänennamen).</span><span class="sxs-lookup"><span data-stu-id="4deba-159">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4deba-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4deba-160">JSON representation</span></span>

<span data-ttu-id="4deba-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4deba-161">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
