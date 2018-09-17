# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="d1dd0-101">Ressourcentyp userSecurityState</span><span class="sxs-lookup"><span data-stu-id="d1dd0-101">userSecurityState resource type</span></span>

<span data-ttu-id="d1dd0-102">Enthält Zustandsinformationen über das Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-102">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="d1dd0-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1dd0-103">Properties</span></span>

| <span data-ttu-id="d1dd0-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1dd0-104">Property</span></span>   | <span data-ttu-id="d1dd0-105">Typ</span><span class="sxs-lookup"><span data-stu-id="d1dd0-105">Type</span></span> |<span data-ttu-id="d1dd0-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1dd0-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1dd0-107">aadUserId</span><span class="sxs-lookup"><span data-stu-id="d1dd0-107">aadUserId</span></span>|<span data-ttu-id="d1dd0-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-108">String</span></span>|<span data-ttu-id="d1dd0-109">AAD-Benutzer-Objektbezeichner (GUID) -stellt die physische/multi-Konto-Benutzerentität dar.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-109">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="d1dd0-110">accountName</span><span class="sxs-lookup"><span data-stu-id="d1dd0-110">accountName</span></span>|<span data-ttu-id="d1dd0-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-111">String</span></span>|<span data-ttu-id="d1dd0-112">Kontoname des Benutzerkontos (ohne Active Directory-Domäne oder DNS-Domäne) - (auch bezeichnet als `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="d1dd0-112">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="d1dd0-113">Domänname</span><span class="sxs-lookup"><span data-stu-id="d1dd0-113">domainName</span></span>|<span data-ttu-id="d1dd0-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-114">String</span></span>|<span data-ttu-id="d1dd0-115">NetBIOS/Active Directory-Domäne des Benutzerkontos (d.h., im Format Domäne\Konto).</span><span class="sxs-lookup"><span data-stu-id="d1dd0-115">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="d1dd0-116">emailRole</span><span class="sxs-lookup"><span data-stu-id="d1dd0-116">emailRole</span></span>|<span data-ttu-id="d1dd0-117">emailRole</span><span class="sxs-lookup"><span data-stu-id="d1dd0-117">emailRole</span></span>|<span data-ttu-id="d1dd0-118">Für E-Mail-bezogene Warnungen - die E-Mail-'Rolle' des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-118">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="d1dd0-119">Mögliche Werte sind: `unknown`, `sender` und `recipient`.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-119">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="d1dd0-120">isVpn</span><span class="sxs-lookup"><span data-stu-id="d1dd0-120">isVpn</span></span>|<span data-ttu-id="d1dd0-121">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d1dd0-121">Boolean</span></span>|<span data-ttu-id="d1dd0-122">Gibt an, ob der Benutzer über ein VPN angemeldet ist.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-122">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="d1dd0-123">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="d1dd0-123">logonDateTime</span></span>|<span data-ttu-id="d1dd0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1dd0-124">DateTimeOffset</span></span>|<span data-ttu-id="d1dd0-125">Zeitpunkt, an dem die Anmeldung stattgefunden hat.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-125">Time at which the sign-in occurred.</span></span> <span data-ttu-id="d1dd0-126">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d1dd0-127">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d1dd0-128">logonId</span><span class="sxs-lookup"><span data-stu-id="d1dd0-128">logonId</span></span>|<span data-ttu-id="d1dd0-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-129">String</span></span>|<span data-ttu-id="d1dd0-130">Benutzer-Anmelde-ID.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-130">User sign-in ID.</span></span>|
|<span data-ttu-id="d1dd0-131">logonIp</span><span class="sxs-lookup"><span data-stu-id="d1dd0-131">logonIp</span></span>|<span data-ttu-id="d1dd0-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-132">String</span></span>|<span data-ttu-id="d1dd0-133">Die IP-Adresse, von der die Anmelde-Anforderung stammt.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-133">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="d1dd0-134">logonLocation</span><span class="sxs-lookup"><span data-stu-id="d1dd0-134">logonLocation</span></span>|<span data-ttu-id="d1dd0-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-135">String</span></span>|<span data-ttu-id="d1dd0-136">Der Speicherort (nach Zuordnung der IP-Adresse), mit dem das Benutzer-Anmelde-Ereignis zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-136">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="d1dd0-137">logonType</span><span class="sxs-lookup"><span data-stu-id="d1dd0-137">logonType</span></span>|<span data-ttu-id="d1dd0-138">logonType</span><span class="sxs-lookup"><span data-stu-id="d1dd0-138">logonType</span></span>|<span data-ttu-id="d1dd0-139">Anmeldemethode des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-139">Method of user sign in.</span></span> <span data-ttu-id="d1dd0-140">Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-140">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="d1dd0-141">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1dd0-141">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="d1dd0-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-142">String</span></span>|<span data-ttu-id="d1dd0-143">Active Directory (lokal) Sicherheitsbezeichner (SID) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-143">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="d1dd0-144">riskScore</span><span class="sxs-lookup"><span data-stu-id="d1dd0-144">riskScore</span></span>|<span data-ttu-id="d1dd0-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-145">String</span></span>|<span data-ttu-id="d1dd0-146">Vom Anbieter generierte/berechnete Risikobewertung des Benutzerkontos.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-146">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="d1dd0-147">Empfohlener Wertebereich von 0-1, was einem Prozentsatz entspricht.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-147">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="d1dd0-148">userAccountType</span><span class="sxs-lookup"><span data-stu-id="d1dd0-148">userAccountType</span></span>|<span data-ttu-id="d1dd0-149">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="d1dd0-149">userAccountSecurityType</span></span>|<span data-ttu-id="d1dd0-150">Typ des Benutzerkontos (Gruppenmitgliedschaft) nach Windows-Definition.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-150">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="d1dd0-151">Mögliche Werte: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-151">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="d1dd0-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d1dd0-152">userPrincipalName</span></span>|<span data-ttu-id="d1dd0-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1dd0-153">String</span></span>|<span data-ttu-id="d1dd0-154">Benutzer-Anmeldename - Internetformat: (Benutzerkontoname) @(Benutzerkonto-DNS-Domänenname).</span><span class="sxs-lookup"><span data-stu-id="d1dd0-154">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1dd0-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1dd0-155">JSON representation</span></span>

<span data-ttu-id="d1dd0-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1dd0-156">The following is a JSON representation of the resource.</span></span>

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
