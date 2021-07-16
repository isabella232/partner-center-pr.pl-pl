---
title: Lista zapytań systemowych dotyczących dostępu programowego szczegółowych informacji o partnerach
description: Dowiedz się więcej o zapytaniach systemowych, których można używać do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376645"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a><span data-ttu-id="f4b81-103">Lista zapytań systemowych dotyczących dostępu programowego szczegółowych informacji o partnerach</span><span class="sxs-lookup"><span data-stu-id="f4b81-103">List of system queries for partner insights programmatic access</span></span>

<span data-ttu-id="f4b81-104">Następujące zapytania systemowe mogą być używane w interfejsie [API tworzenia raportu](insights-programmatic-access-paradigm.md#create-report-api) bezpośrednio z queryId.</span><span class="sxs-lookup"><span data-stu-id="f4b81-104">The following system queries can be used in the [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directly with a QueryId.</span></span> <span data-ttu-id="f4b81-105">Zapytania systemowe są podobne do raportów eksportu w Partner Center przez sześć miesięcy (6 mln).</span><span class="sxs-lookup"><span data-stu-id="f4b81-105">The system queries are like the export reports in Partner Center for a six-month (6M) computation period.</span></span>

<span data-ttu-id="f4b81-106">Aby uzyskać więcej informacji na temat nazw kolumn, atrybutów i opisu, zapoznaj się z [definicjami danych](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="f4b81-106">For more details on the column names, attributes, and description, please refer to the [Data Definitions](insights-data-definitions.md)</span></span>

<span data-ttu-id="f4b81-107">Poniższe sekcje zawierają zapytania dotyczące raportów dla różnych raportów.</span><span class="sxs-lookup"><span data-stu-id="f4b81-107">The following sections provide report queries for various reports.</span></span>

## <a name="customers"></a><span data-ttu-id="f4b81-108">Klienci</span><span class="sxs-lookup"><span data-stu-id="f4b81-108">Customers</span></span>

<span data-ttu-id="f4b81-109">Raport Klienci z ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-109">The Customers report for the last six months</span></span>

<span data-ttu-id="f4b81-110">Identyfikator zapytania: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span><span class="sxs-lookup"><span data-stu-id="f4b81-110">Query ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-111">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-111">Report query</span></span>
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a><span data-ttu-id="f4b81-112">Subskrypcje stanowisk i przychód</span><span class="sxs-lookup"><span data-stu-id="f4b81-112">Seats Subscriptions and Revenue</span></span>

<span data-ttu-id="f4b81-113">Stanowiska, subskrypcje i raport przychodów z ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-113">Seats, subscriptions, and revenue report for the last six months</span></span>

<span data-ttu-id="f4b81-114">Identyfikator zapytania: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span><span class="sxs-lookup"><span data-stu-id="f4b81-114">Query ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-115">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-115">Report query</span></span>

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a><span data-ttu-id="f4b81-116">Profil partnera</span><span class="sxs-lookup"><span data-stu-id="f4b81-116">Partner Profile</span></span>

<span data-ttu-id="f4b81-117">Profilowanie danych</span><span class="sxs-lookup"><span data-stu-id="f4b81-117">Profile data</span></span>

<span data-ttu-id="f4b81-118">Identyfikator zapytania: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span><span class="sxs-lookup"><span data-stu-id="f4b81-118">Query ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-119">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-119">Report query</span></span>

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a><span data-ttu-id="f4b81-120">Użycie platformy Azure</span><span class="sxs-lookup"><span data-stu-id="f4b81-120">Azure Usage</span></span>

<span data-ttu-id="f4b81-121">Raport AzureUsage z ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-121">AzureUsage report for the last six months</span></span>

<span data-ttu-id="f4b81-122">Identyfikator zapytania: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span><span class="sxs-lookup"><span data-stu-id="f4b81-122">Query ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-123">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-123">Report query</span></span>

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a><span data-ttu-id="f4b81-124">Office Użycia</span><span class="sxs-lookup"><span data-stu-id="f4b81-124">Office Usage</span></span>

<span data-ttu-id="f4b81-125">Raport OfficeUsage z ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-125">OfficeUsage report for the last six months</span></span>

<span data-ttu-id="f4b81-126">Identyfikator zapytania: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span><span class="sxs-lookup"><span data-stu-id="f4b81-126">Query ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-127">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-127">Report query</span></span>

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a><span data-ttu-id="f4b81-128">Użycie usługi Dynamics</span><span class="sxs-lookup"><span data-stu-id="f4b81-128">Dynamics Usage</span></span>

<span data-ttu-id="f4b81-129">Raport DynamicsUsage z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-129">DynamicsUsage report for six months</span></span>

<span data-ttu-id="f4b81-130">Identyfikator zapytania: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span><span class="sxs-lookup"><span data-stu-id="f4b81-130">Query ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-131">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-131">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a><span data-ttu-id="f4b81-132">Użycie usługi Power BI</span><span class="sxs-lookup"><span data-stu-id="f4b81-132">Power BI usage</span></span>

<span data-ttu-id="f4b81-133">Raport usługi PowerBIUsage z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-133">PowerBIUsage report for six months</span></span>

<span data-ttu-id="f4b81-134">Identyfikator zapytania: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span><span class="sxs-lookup"><span data-stu-id="f4b81-134">Query ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-135">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-135">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a><span data-ttu-id="f4b81-136">Użycie usług EMS</span><span class="sxs-lookup"><span data-stu-id="f4b81-136">EMS Usage</span></span>

<span data-ttu-id="f4b81-137">Raport EMSUsage przez sześć miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-137">EMSUsage report for six months</span></span>

<span data-ttu-id="f4b81-138">Identyfikator zapytania: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span><span class="sxs-lookup"><span data-stu-id="f4b81-138">Query ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-139">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-139">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a><span data-ttu-id="f4b81-140">Raport wymagań w zakresie wydajności kompetencji</span><span class="sxs-lookup"><span data-stu-id="f4b81-140">Competency Performance requirement report</span></span>

<span data-ttu-id="f4b81-141">Raport CompetencyPeformanceRequirement z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-141">CompetencyPeformanceRequirement report for six months</span></span>

<span data-ttu-id="f4b81-142">Identyfikator zapytania: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span><span class="sxs-lookup"><span data-stu-id="f4b81-142">Query ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-143">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-143">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a><span data-ttu-id="f4b81-144">Wydajność odsprzedawcy produktów w chmurze</span><span class="sxs-lookup"><span data-stu-id="f4b81-144">Cloud products reseller performance</span></span>

### <a name="report-description"></a><span data-ttu-id="f4b81-145">Opis raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-145">Report description</span></span>

<span data-ttu-id="f4b81-146">Raport CloudProductsResellerPerformance z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-146">CloudProductsResellerPerformance report for six months</span></span>

<span data-ttu-id="f4b81-147">Identyfikator zapytania: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span><span class="sxs-lookup"><span data-stu-id="f4b81-147">Query ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-148">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-148">Report query</span></span>

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a><span data-ttu-id="f4b81-149">Proporcjonalność do odnawiania umowy CLAS</span><span class="sxs-lookup"><span data-stu-id="f4b81-149">CLAS Agreement Renewal propensity</span></span>

<span data-ttu-id="f4b81-150">Raport CLASAgreementRenewalsPropensity z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-150">CLASAgreementRenewalsPropensity report for six months</span></span>

<span data-ttu-id="f4b81-151">Identyfikator zapytania: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span><span class="sxs-lookup"><span data-stu-id="f4b81-151">Query ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-152">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-152">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a><span data-ttu-id="f4b81-153">Clas Azure propensity</span><span class="sxs-lookup"><span data-stu-id="f4b81-153">CLAS Azure propensity</span></span>

<span data-ttu-id="f4b81-154">Raport CLASAzurePropensity przez sześć miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-154">CLASAzurePropensity report for six months</span></span>

<span data-ttu-id="f4b81-155">Identyfikator zapytania: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span><span class="sxs-lookup"><span data-stu-id="f4b81-155">Query ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-156">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-156">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a><span data-ttu-id="f4b81-157">Clas D365 propensity</span><span class="sxs-lookup"><span data-stu-id="f4b81-157">CLAS D365 propensity</span></span>

<span data-ttu-id="f4b81-158">Raport CLASD365Propensity dla sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-158">CLASD365Propensity report for six months</span></span>

<span data-ttu-id="f4b81-159">Identyfikator zapytania: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span><span class="sxs-lookup"><span data-stu-id="f4b81-159">Query ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-160">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-160">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a><span data-ttu-id="f4b81-161">CLAS M365 propensity</span><span class="sxs-lookup"><span data-stu-id="f4b81-161">CLAS M365 propensity</span></span>

<span data-ttu-id="f4b81-162">Raport CLASM365Propensity dla sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-162">CLASM365Propensity report for six months</span></span>

<span data-ttu-id="f4b81-163">Identyfikator zapytania: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span><span class="sxs-lookup"><span data-stu-id="f4b81-163">Query ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-164">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-164">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a><span data-ttu-id="f4b81-165">Teams Użycie aplikacji 3P</span><span class="sxs-lookup"><span data-stu-id="f4b81-165">Teams Usage 3P Apps</span></span>

<span data-ttu-id="f4b81-166">Raport TeamsUsage3PApps przez sześć miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-166">TeamsUsage3PApps report for six months</span></span>

<span data-ttu-id="f4b81-167">Identyfikator zapytania: `42d287be-cc76-4109-a066-f3140ad97fe2`</span><span class="sxs-lookup"><span data-stu-id="f4b81-167">Query ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-168">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-168">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a><span data-ttu-id="f4b81-169">Teams obciążenia użycia</span><span class="sxs-lookup"><span data-stu-id="f4b81-169">Teams usage workload</span></span>

<span data-ttu-id="f4b81-170">Raport TeamsUsageWorkload przez sześć miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-170">TeamsUsageWorkload report for six months</span></span>

<span data-ttu-id="f4b81-171">Identyfikator zapytania: `817fe875-acb0-4c45-9201-b7a35a60235a`</span><span class="sxs-lookup"><span data-stu-id="f4b81-171">Query ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-172">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-172">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a><span data-ttu-id="f4b81-173">Teams użycia i połączenia</span><span class="sxs-lookup"><span data-stu-id="f4b81-173">Teams usage meetings and calls</span></span>

<span data-ttu-id="f4b81-174">Raport TeamsUsageMeetingsAndCalls przez sześć miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-174">TeamsUsageMeetingsAndCalls report for six months</span></span>

<span data-ttu-id="f4b81-175">Identyfikator zapytania: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span><span class="sxs-lookup"><span data-stu-id="f4b81-175">Query ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-176">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-176">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a><span data-ttu-id="f4b81-177">Historia podsumowania kompetencji</span><span class="sxs-lookup"><span data-stu-id="f4b81-177">Competency summary history</span></span>

<span data-ttu-id="f4b81-178">Raport CompetencySummaryHistory z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-178">CompetencySummaryHistory report for six months</span></span>

<span data-ttu-id="f4b81-179">Identyfikator zapytania: `fddab2aa-523d-47f6-90fe-588557306db4`</span><span class="sxs-lookup"><span data-stu-id="f4b81-179">Query ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-180">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-180">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a><span data-ttu-id="f4b81-181">Ukończenie szkolenia</span><span class="sxs-lookup"><span data-stu-id="f4b81-181">Training completion</span></span>

<span data-ttu-id="f4b81-182">Raport ukończenia szkolenia z sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-182">Training Completions report for six months</span></span>

<span data-ttu-id="f4b81-183">Identyfikator zapytania: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span><span class="sxs-lookup"><span data-stu-id="f4b81-183">Query ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-184">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-184">Report query</span></span>

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a><span data-ttu-id="f4b81-185">Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="f4b81-185">Microsoft Learn</span></span>

<span data-ttu-id="f4b81-186">Microsoft Learn raportu z ostatnich sześciu miesięcy</span><span class="sxs-lookup"><span data-stu-id="f4b81-186">Microsoft Learn report for the last six months</span></span>

<span data-ttu-id="f4b81-187">Identyfikator zapytania: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span><span class="sxs-lookup"><span data-stu-id="f4b81-187">Query ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span></span>

### <a name="report-query"></a><span data-ttu-id="f4b81-188">Zapytanie raportu</span><span class="sxs-lookup"><span data-stu-id="f4b81-188">Report query</span></span>

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="f4b81-189">Następne kroki</span><span class="sxs-lookup"><span data-stu-id="f4b81-189">Next steps</span></span>

- [<span data-ttu-id="f4b81-190">Interfejsy API do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów</span><span class="sxs-lookup"><span data-stu-id="f4b81-190">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
- [<span data-ttu-id="f4b81-191">Przykładowa aplikacja do uzyskiwania dostępu do danych analitycznych szczegółowych informacji partnerów</span><span class="sxs-lookup"><span data-stu-id="f4b81-191">Sample application for accessing partner insights analytics data</span></span>](insights-programmatic-sample-application.md)