# <a name="auditactor-resource-type"></a><span data-ttu-id="1993c-101">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1993c-101">auditActor resource type</span></span>

> <span data-ttu-id="1993c-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1993c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1993c-103">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="1993c-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="1993c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1993c-104">Properties</span></span>
|<span data-ttu-id="1993c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1993c-105">Property</span></span>|<span data-ttu-id="1993c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="1993c-106">Type</span></span>|<span data-ttu-id="1993c-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1993c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1993c-108">type</span><span class="sxs-lookup"><span data-stu-id="1993c-108">type</span></span>|<span data-ttu-id="1993c-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-109">String</span></span>|<span data-ttu-id="1993c-110">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="1993c-110">Actor Type.</span></span>|
|<span data-ttu-id="1993c-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1993c-111">permissions</span></span>|<span data-ttu-id="1993c-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1993c-112">String collection</span></span>|<span data-ttu-id="1993c-113">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="1993c-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="1993c-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="1993c-114">userPermissions</span></span>|<span data-ttu-id="1993c-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1993c-115">String collection</span></span>|<span data-ttu-id="1993c-116">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="1993c-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="1993c-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="1993c-117">applicationId</span></span>|<span data-ttu-id="1993c-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-118">String</span></span>|<span data-ttu-id="1993c-119">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="1993c-119">AAD Application Id.</span></span>|
|<span data-ttu-id="1993c-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1993c-120">applicationDisplayName</span></span>|<span data-ttu-id="1993c-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-121">String</span></span>|<span data-ttu-id="1993c-122">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="1993c-122">Name of the Application.</span></span>|
|<span data-ttu-id="1993c-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1993c-123">userPrincipalName</span></span>|<span data-ttu-id="1993c-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-124">String</span></span>|<span data-ttu-id="1993c-125">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="1993c-125">User principal name (UPN)</span></span>|
|<span data-ttu-id="1993c-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1993c-126">servicePrincipalName</span></span>|<span data-ttu-id="1993c-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-127">String</span></span>|<span data-ttu-id="1993c-128">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="1993c-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="1993c-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1993c-129">ipAddress</span></span>|<span data-ttu-id="1993c-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-130">String</span></span>|<span data-ttu-id="1993c-131">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="1993c-131">IPAddress.</span></span>|
|<span data-ttu-id="1993c-132">userId</span><span class="sxs-lookup"><span data-stu-id="1993c-132">userID</span></span>|<span data-ttu-id="1993c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1993c-133">String</span></span>|<span data-ttu-id="1993c-134">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="1993c-134">User ID</span></span>|

## <a name="relationships"></a><span data-ttu-id="1993c-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1993c-135">Relationships</span></span>
<span data-ttu-id="1993c-136">Keine</span><span class="sxs-lookup"><span data-stu-id="1993c-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1993c-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1993c-137">JSON Representation</span></span>
<span data-ttu-id="1993c-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1993c-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "permissions": [
    "String"
  ],
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```



