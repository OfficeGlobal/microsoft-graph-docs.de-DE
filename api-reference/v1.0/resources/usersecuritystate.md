---
title: Ressourcentyp userSecurityState
description: Statusinformationen über das Benutzerkonto enthält.
ms.openlocfilehash: dbb4b6600cc11a75c84f2f0b233535d012309f88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018544"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="60f04-103">Ressourcentyp userSecurityState</span><span class="sxs-lookup"><span data-stu-id="60f04-103">userSecurityState resource type</span></span>

<span data-ttu-id="60f04-104">Statusinformationen über das Benutzerkonto enthält.</span><span class="sxs-lookup"><span data-stu-id="60f04-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="60f04-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60f04-105">Properties</span></span>

| <span data-ttu-id="60f04-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60f04-106">Property</span></span>   | <span data-ttu-id="60f04-107">Typ</span><span class="sxs-lookup"><span data-stu-id="60f04-107">Type</span></span> |<span data-ttu-id="60f04-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60f04-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60f04-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="60f04-109">aadUserId</span></span>|<span data-ttu-id="60f04-110">String</span><span class="sxs-lookup"><span data-stu-id="60f04-110">String</span></span>|<span data-ttu-id="60f04-111">AAD Benutzer Objekt-ID (GUID) - die physische/multi-account Benutzerentität darstellt.</span><span class="sxs-lookup"><span data-stu-id="60f04-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="60f04-112">accountName</span><span class="sxs-lookup"><span data-stu-id="60f04-112">accountName</span></span>|<span data-ttu-id="60f04-113">String</span><span class="sxs-lookup"><span data-stu-id="60f04-113">String</span></span>|<span data-ttu-id="60f04-114">Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch als bezeichnet `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="60f04-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="60f04-115">Domänname</span><span class="sxs-lookup"><span data-stu-id="60f04-115">domainName</span></span>|<span data-ttu-id="60f04-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60f04-116">String</span></span>|<span data-ttu-id="60f04-117">NetBIOS/Active Directory-Domäne des Benutzerkontos (d. h., im Format Domäne\Konto).</span><span class="sxs-lookup"><span data-stu-id="60f04-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="60f04-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="60f04-118">emailRole</span></span>|<span data-ttu-id="60f04-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="60f04-119">emailRole</span></span>|<span data-ttu-id="60f04-120">Für e-Mail-bezogene Alerts - des Benutzerkontos e-Mail 'Role'.</span><span class="sxs-lookup"><span data-stu-id="60f04-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="60f04-121">Mögliche Werte sind: `unknown`, `sender` und `recipient`.</span><span class="sxs-lookup"><span data-stu-id="60f04-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="60f04-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="60f04-122">isVpn</span></span>|<span data-ttu-id="60f04-123">Boolesch</span><span class="sxs-lookup"><span data-stu-id="60f04-123">Boolean</span></span>|<span data-ttu-id="60f04-124">Gibt an, ob der Benutzer über ein VPN angemeldet.</span><span class="sxs-lookup"><span data-stu-id="60f04-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="60f04-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="60f04-125">logonDateTime</span></span>|<span data-ttu-id="60f04-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60f04-126">DateTimeOffset</span></span>|<span data-ttu-id="60f04-127">Zeitpunkt der Anmeldung bei der aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="60f04-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="60f04-128">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="60f04-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="60f04-129">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="60f04-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="60f04-130">logonId</span><span class="sxs-lookup"><span data-stu-id="60f04-130">logonId</span></span>|<span data-ttu-id="60f04-131">String</span><span class="sxs-lookup"><span data-stu-id="60f04-131">String</span></span>|<span data-ttu-id="60f04-132">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="60f04-132">User sign-in ID.</span></span>|
|<span data-ttu-id="60f04-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="60f04-133">logonIp</span></span>|<span data-ttu-id="60f04-134">String</span><span class="sxs-lookup"><span data-stu-id="60f04-134">String</span></span>|<span data-ttu-id="60f04-135">IP-Adresse, die von die Anforderung-Anmeldung stammt.</span><span class="sxs-lookup"><span data-stu-id="60f04-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="60f04-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="60f04-136">logonLocation</span></span>|<span data-ttu-id="60f04-137">String</span><span class="sxs-lookup"><span data-stu-id="60f04-137">String</span></span>|<span data-ttu-id="60f04-138">Speicherort (nach Zuordnung von IP-Adresse) ein Benutzer anmelden Ereignis von diesem Benutzer zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="60f04-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="60f04-139">logonType</span><span class="sxs-lookup"><span data-stu-id="60f04-139">logonType</span></span>|<span data-ttu-id="60f04-140">logonType</span><span class="sxs-lookup"><span data-stu-id="60f04-140">logonType</span></span>|<span data-ttu-id="60f04-141">-Methode des Benutzers anmelden.</span><span class="sxs-lookup"><span data-stu-id="60f04-141">Method of user sign in.</span></span> <span data-ttu-id="60f04-142">Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.</span><span class="sxs-lookup"><span data-stu-id="60f04-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="60f04-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="60f04-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="60f04-144">String</span><span class="sxs-lookup"><span data-stu-id="60f04-144">String</span></span>|<span data-ttu-id="60f04-145">Active Directory (lokal) Sicherheits-ID (SID) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="60f04-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="60f04-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="60f04-146">riskScore</span></span>|<span data-ttu-id="60f04-147">String</span><span class="sxs-lookup"><span data-stu-id="60f04-147">String</span></span>|<span data-ttu-id="60f04-148">Provider-generiert/berechnet Risiko Bewertung des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="60f04-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="60f04-149">Empfohlene Wertebereich von 0 bis 1, die den Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="60f04-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="60f04-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="60f04-150">userAccountType</span></span>|<span data-ttu-id="60f04-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="60f04-151">userAccountSecurityType</span></span>|<span data-ttu-id="60f04-152">Typ des Benutzerkontos (Gruppenmitgliedschaft) pro Windows-Definition.</span><span class="sxs-lookup"><span data-stu-id="60f04-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="60f04-153">Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.</span><span class="sxs-lookup"><span data-stu-id="60f04-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="60f04-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="60f04-154">userPrincipalName</span></span>|<span data-ttu-id="60f04-155">String</span><span class="sxs-lookup"><span data-stu-id="60f04-155">String</span></span>|<span data-ttu-id="60f04-156">Benutzer-Anmeldename - Internetformat: (Benutzerkontonamen) @(Konto DNS-Domänennamen).</span><span class="sxs-lookup"><span data-stu-id="60f04-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60f04-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60f04-157">JSON representation</span></span>

<span data-ttu-id="60f04-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60f04-158">The following is a JSON representation of the resource.</span></span>

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
