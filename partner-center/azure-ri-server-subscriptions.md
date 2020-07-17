---
title: Резервирования Azure & серверные подписки
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Узнайте о возможностях поставщиков облачных решений по приобретению, подготовке и управлению резервированиями Azure и серверными подписками для клиентов.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b804c76428b0d1f699874b48f7a884161aebcdd
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435713"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="d2378-103">Получение, инициализация, & управление зарезервированными экземплярами виртуальных машин Azure (RI) и серверными подписками для клиентов</span><span class="sxs-lookup"><span data-stu-id="d2378-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="d2378-104">Область применения:</span><span class="sxs-lookup"><span data-stu-id="d2378-104">Applies to:</span></span>

- <span data-ttu-id="d2378-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="d2378-105">Partner Center</span></span>

<span data-ttu-id="d2378-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="d2378-106">**Appropriate roles**</span></span>

- <span data-ttu-id="d2378-107">Агент по администрированию</span><span class="sxs-lookup"><span data-stu-id="d2378-107">Admin agent</span></span>
- <span data-ttu-id="d2378-108">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d2378-108">Global admin</span></span>
- <span data-ttu-id="d2378-109">Агент службы технической поддержки</span><span class="sxs-lookup"><span data-stu-id="d2378-109">Helpdesk agent</span></span>
- <span data-ttu-id="d2378-110">Агент по продажам</span><span class="sxs-lookup"><span data-stu-id="d2378-110">Sales agent</span></span>
- <span data-ttu-id="d2378-111">Администратор управления пользователями</span><span class="sxs-lookup"><span data-stu-id="d2378-111">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="d2378-112">Общие сведения о резервированиях в Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-112">What are Azure Reservations?</span></span>

<span data-ttu-id="d2378-113">Резервирование Azure помогает экономить деньги за счет предварительной оплаты за один или три года виртуальной машины, объема вычислений базы данных SQL, Azure Cosmos DB пропускной способности или других ресурсов Azure.</span><span class="sxs-lookup"><span data-stu-id="d2378-113">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="d2378-114">Предоплата позволяет получить скидку на использование ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d2378-114">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="d2378-115">Резервирования могут значительно снизить объем виртуальной машины, вычисление базы данных SQL, Azure Cosmos DB и другие затраты на ресурсы до 72% по сравнению с ценами оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="d2378-115">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="d2378-116">Резервирования предоставляют скидку при выставлении счетов и не влияют на состояние выполнения ваших ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d2378-116">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="d2378-117">Дополнительные сведения см. в статье [что такое резервирование Azure?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="d2378-117">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="d2378-118">Почему клиенты должны приобрести резервирование?</span><span class="sxs-lookup"><span data-stu-id="d2378-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="d2378-119">Если у клиентов есть виртуальные машины, Azure Cosmos DB или базы данных SQL, работающие в течение длительного периода времени, приобретение резервирования дает им наиболее экономичный вариант.</span><span class="sxs-lookup"><span data-stu-id="d2378-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="d2378-120">Например, если клиент непрерывно запускает четыре экземпляра службы без резервирования, плата взимается по тарифам с оплатой по мере использования.</span><span class="sxs-lookup"><span data-stu-id="d2378-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="d2378-121">Если они приобретают резервирование для этих ресурсов, они незамедлительно получают скидку на резервирование.</span><span class="sxs-lookup"><span data-stu-id="d2378-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="d2378-122">К ресурсам больше не будут применяться ставки оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="d2378-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="d2378-123">Новое интересное предложение Azure в программе CSP</span><span class="sxs-lookup"><span data-stu-id="d2378-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="d2378-124">Выполнив резервирование Azure и серверные подписки на свою программу CSP, корпорация Майкрософт лучше позволяет своим партнерам решать быстро растущие потребности клиентов, обеспечивая более экономичные решения для поддержки строго предсказуемых и устойчивых облачных рабочих нагрузок.</span><span class="sxs-lookup"><span data-stu-id="d2378-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="d2378-125">Программа CSP позволяет партнерам получать, подготавливать резервирования Azure и серверные подписки и управлять ими от имени коммерческих клиентов через центр партнеров Майкрософт и портал Azure.</span><span class="sxs-lookup"><span data-stu-id="d2378-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="d2378-126">Мы даже предоставляем партнерам в нашей программе CSP сведения о том, как можно приобрести резервирования Azure.</span><span class="sxs-lookup"><span data-stu-id="d2378-126">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="d2378-127">Партнеры CSP могут [купить резервирование Azure от имени клиента](azure-reservations-buying.md) или [позволить клиенту покупать собственные резервирования](give-customers-permission.md) из предыдущей подписки Azure, приобретенной для них партнером.</span><span class="sxs-lookup"><span data-stu-id="d2378-127">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="d2378-128">Резервирование Azure предоставляет клиентам гибкие возможности виртуализации для широкого спектра вычислительных решений, включая разработку и тестирование, запуск приложений и расширение центра обработки данных.</span><span class="sxs-lookup"><span data-stu-id="d2378-128">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="d2378-129">С [Azure reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) , например, коммерческие клиенты могут сэкономить до 72% по сравнению с оплатой по мере использования, используя цены на виртуальные машины Azure по мере покупки или "резервирования" — виртуальную машину на 1-или 3-летний период.</span><span class="sxs-lookup"><span data-stu-id="d2378-129">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="d2378-130">Клиенты с Windows Server, которые уже успели оценить преимущества гибридного использования Azure и поддержки Software Assurance, могут сэкономить до 80% по сравнению с моделью оплаты по мере использования.</span><span class="sxs-lookup"><span data-stu-id="d2378-130">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="d2378-131">Благодаря несовпадающей комбинации привлекательной цены и несовпадающей гибкости развертывания клиенты увидят лучшее общее значение при выборе резервирования Azure:</span><span class="sxs-lookup"><span data-stu-id="d2378-131">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="d2378-132">Резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-132">Azure reservations</span></span>

- <span data-ttu-id="d2378-133">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="d2378-133">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="d2378-134">Резервирования базы данных SQL</span><span class="sxs-lookup"><span data-stu-id="d2378-134">SQL DB Reservations</span></span>
- <span data-ttu-id="d2378-135">Управляемый экземпляр SQL</span><span class="sxs-lookup"><span data-stu-id="d2378-135">SQL Managed Instance</span></span>
- <span data-ttu-id="d2378-136">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d2378-136">Azure Cosmos DB</span></span>
- <span data-ttu-id="d2378-137">Хранилище данных SQL Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-137">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="d2378-138">Службы приложений</span><span class="sxs-lookup"><span data-stu-id="d2378-138">App Services</span></span>
- <span data-ttu-id="d2378-139">Azure Databricks резервирования единиц измерения</span><span class="sxs-lookup"><span data-stu-id="d2378-139">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="d2378-140">Управляемые диски</span><span class="sxs-lookup"><span data-stu-id="d2378-140">Managed Disk</span></span>
- <span data-ttu-id="d2378-141">Блочный BLOB-объект</span><span class="sxs-lookup"><span data-stu-id="d2378-141">Block blob</span></span>
- <span data-ttu-id="d2378-142">MySQL</span><span class="sxs-lookup"><span data-stu-id="d2378-142">MySQL</span></span>
- <span data-ttu-id="d2378-143">Обозреватель данных Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-143">Azure Data explorer</span></span>
- <span data-ttu-id="d2378-144">MariaDB</span><span class="sxs-lookup"><span data-stu-id="d2378-144">MariaDB</span></span>
- <span data-ttu-id="d2378-145">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="d2378-145">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="d2378-146">Серверные подписки</span><span class="sxs-lookup"><span data-stu-id="d2378-146">Server subscriptions</span></span>

- <span data-ttu-id="d2378-147">Windows Server</span><span class="sxs-lookup"><span data-stu-id="d2378-147">Windows Server</span></span>
- <span data-ttu-id="d2378-148">Клиентские лицензии службы удаленных рабочих столов (RDS)</span><span class="sxs-lookup"><span data-stu-id="d2378-148">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="d2378-149">SQL Server</span><span class="sxs-lookup"><span data-stu-id="d2378-149">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="d2378-150">Ежегодные подписки независимых поставщиков по Linux</span><span class="sxs-lookup"><span data-stu-id="d2378-150">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="d2378-151">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="d2378-151">SUSE Linux</span></span>
- <span data-ttu-id="d2378-152">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="d2378-152">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="d2378-153">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="d2378-153">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="d2378-154">Ежегодные подписки ISV</span><span class="sxs-lookup"><span data-stu-id="d2378-154">ISV annual subscriptions</span></span>

- <span data-ttu-id="d2378-155">Решение VMware в Azure от CloudSimple</span><span class="sxs-lookup"><span data-stu-id="d2378-155">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="d2378-156">Начало работы</span><span class="sxs-lookup"><span data-stu-id="d2378-156">Getting started</span></span>

<span data-ttu-id="d2378-157">Чтобы понять, как можно разместить резервирование Azure для клиентов и быстро приступить к работе, мы рекомендуем использовать следующий подход для просмотра материалов о готовности:</span><span class="sxs-lookup"><span data-stu-id="d2378-157">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="d2378-158">Просмотрите обзорную презентацию и сопутствующий вебинар о позиционировании и формировании предложений для клиентов</span><span class="sxs-lookup"><span data-stu-id="d2378-158">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="d2378-159">Изучите руководство по современной коммерции</span><span class="sxs-lookup"><span data-stu-id="d2378-159">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="d2378-160">Изучите раздел "Подписки на Azure RI и серверные подписки: вопросы и ответы"</span><span class="sxs-lookup"><span data-stu-id="d2378-160">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="d2378-161">Ознакомьтесь с информацией об обновлении резервирований Azure и серверных подписок в документе [API Центра партнеров (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="d2378-161">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="d2378-162">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="d2378-162">Resources</span></span>

<span data-ttu-id="d2378-163">Ниже приведен полный список ресурсов, которые помогут вам быстро приступить к работе с резервированиями Azure в Центре партнеров.</span><span class="sxs-lookup"><span data-stu-id="d2378-163">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="d2378-164">Готовность к продажам</span><span class="sxs-lookup"><span data-stu-id="d2378-164">Sales readiness</span></span>

- [<span data-ttu-id="d2378-165">Резервирование Azure и серверные подписки с обзором Преимущество гибридного использования Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-165">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="d2378-166">Листовка</span><span class="sxs-lookup"><span data-stu-id="d2378-166">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="d2378-167">Часто задаваемые вопросы о резервировании Azure для партнеров</span><span class="sxs-lookup"><span data-stu-id="d2378-167">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="d2378-168">Часто задаваемые вопросы о резервировании Azure и базе данных SQL</span><span class="sxs-lookup"><span data-stu-id="d2378-168">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="d2378-169">Клиентская лицензия службы удаленных рабочих столов (RDS) (объявление)</span><span class="sxs-lookup"><span data-stu-id="d2378-169">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="d2378-170">Azure Reserved VM Instances (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="d2378-170">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="d2378-171">Серверные подписки</span><span class="sxs-lookup"><span data-stu-id="d2378-171">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="d2378-172">Общие сведения о базе данных SQL в Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-172">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="d2378-173">Резервирования базы данных SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="d2378-173">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="d2378-174">Azure Cosmos DB (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="d2378-174">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="d2378-175">Управляемый экземпляр SQL (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="d2378-175">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="d2378-176">SUSE и Red Hat Enterprise Linux (портал Azure)</span><span class="sxs-lookup"><span data-stu-id="d2378-176">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="d2378-177">Red Hat Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-177">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="d2378-178">SUSE Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-178">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="d2378-179">Linux в Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-179">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="d2378-180">Общие сведения о ценах на Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-180">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="d2378-181">Калькулятор цен Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-181">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="d2378-182">Azure Databricks резервирования единиц измерения</span><span class="sxs-lookup"><span data-stu-id="d2378-182">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="d2378-183">Прайс-страницы CSP. списки **Microsoft Azure зарезервированные экземпляры** и цены на **программное обеспечение** находятся на странице цен на центр партнеров [& предложения](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="d2378-183">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="d2378-184">Обучение</span><span class="sxs-lookup"><span data-stu-id="d2378-184">Training</span></span>

<span data-ttu-id="d2378-185">Зарегистрируйтесь для просмотра веб- [семинаров о готовности к лицензированию](https://commercial-licensing.eventbuilder.com/FY2019_ALL) и событиях по требованию.</span><span class="sxs-lookup"><span data-stu-id="d2378-185">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="d2378-186">События готовности к лицензированию по требованию включают такие темы:</span><span class="sxs-lookup"><span data-stu-id="d2378-186">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="d2378-187">Веб-службы CSP, Azure CSP и общие обновления лицензирования, включая Azure (Ноябрь 2018)</span><span class="sxs-lookup"><span data-stu-id="d2378-187">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="d2378-188">Зарезервированная емкость базы данных SQL & гибкость размера экземпляра (2018 августа)</span><span class="sxs-lookup"><span data-stu-id="d2378-188">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="d2378-189">Серверные подписки в CSP (Июль 2018)</span><span class="sxs-lookup"><span data-stu-id="d2378-189">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="d2378-190">Обзор резервирования Azure в CSP (Май 2018)</span><span class="sxs-lookup"><span data-stu-id="d2378-190">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="d2378-191">Другое полезное обучение включает в себя [модуль лицензирования Azure в университете Partner](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="d2378-191">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="d2378-192">Операции</span><span class="sxs-lookup"><span data-stu-id="d2378-192">Operations</span></span>

- <span data-ttu-id="d2378-193">[Руководство по современным коммерческим операциям](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (Обновлено): исчерпывающее руководство по ключевым политикам и рабочим аспектам, таким как соглашения, упорядочение по центру партнеров, счета, сведения о прайс-листах, поощрения, файл СВЕРКИ, API/SDK, песочница и общие службы партнеров Azure.</span><span class="sxs-lookup"><span data-stu-id="d2378-193">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="d2378-194">Последние сведения о доступности предложений в странах и матрица валют для клиентов</span><span class="sxs-lookup"><span data-stu-id="d2378-194">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="d2378-195">Продажа Microsoft Azure Reserved Instances</span><span class="sxs-lookup"><span data-stu-id="d2378-195">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="d2378-196">Приобретение резервирований Microsoft Azure от лица клиентов</span><span class="sxs-lookup"><span data-stu-id="d2378-196">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="d2378-197">Управление резервированиями Azure от лица клиентов</span><span class="sxs-lookup"><span data-stu-id="d2378-197">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="d2378-198">Выставление счетов за резервирования Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-198">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="d2378-199">Размеры виртуальных машин для максимального использования резервирования</span><span class="sxs-lookup"><span data-stu-id="d2378-199">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="d2378-200">API центра партнеров (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="d2378-200">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="d2378-201">Службы удаленных рабочих столов</span><span class="sxs-lookup"><span data-stu-id="d2378-201">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="d2378-202">Преимущество гибридного использования Azure</span><span class="sxs-lookup"><span data-stu-id="d2378-202">Azure Hybrid Benefit</span></span>

<span data-ttu-id="d2378-203">[Преимущество гибридного использования Azure](https://azure.microsoft.com/pricing/hybrid-benefit) помогает получить дополнительную прибыль от лицензий на Windows Server и сэкономить до \*47 процентов на виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="d2378-203">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="d2378-204">Это преимущество можно использовать с лицензиями Windows Server Datacenter и Standard Edition, зарегистрированными в программе Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="d2378-204">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="d2378-205">В зависимости от выпуска вы можете преобразовывать или повторно использовать лицензии для запуска виртуальных машин Windows Server в Azure и платить за нижнюю базовую частоту вычислений (тарифы виртуальных машин Linux).</span><span class="sxs-lookup"><span data-stu-id="d2378-205">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="d2378-206">См. также [Преимущество гибридного использования Azure — вопросы и ответы](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="d2378-206">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="d2378-207">\* Фактическая экономия может варьироваться в зависимости от региона, типа экземпляра или использования.</span><span class="sxs-lookup"><span data-stu-id="d2378-207">\*Actual savings may vary based on region, instance type, or usage.</span></span>
