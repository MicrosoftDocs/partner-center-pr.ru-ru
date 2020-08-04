---
title: Поля для CSV-файла для импорта нескольких пользователей для учетной записи клиента
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, создайте файл значений с разделителями-запятыми (CSV) с соответствующими полями.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528188"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="f3f38-103">Добавление нескольких пользователей в учетную запись клиента путем создания CSV-файла</span><span class="sxs-lookup"><span data-stu-id="f3f38-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="f3f38-104">**Относится к**</span><span class="sxs-lookup"><span data-stu-id="f3f38-104">**Applies to**</span></span>

- <span data-ttu-id="f3f38-105">Центр партнеров</span><span class="sxs-lookup"><span data-stu-id="f3f38-105">Partner Center</span></span>

<span data-ttu-id="f3f38-106">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="f3f38-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f3f38-107">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f3f38-107">Global admin</span></span>

<span data-ttu-id="f3f38-108">Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="f3f38-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="f3f38-109">Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.</span><span class="sxs-lookup"><span data-stu-id="f3f38-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="f3f38-110">Требования к файлу данных</span><span class="sxs-lookup"><span data-stu-id="f3f38-110">Data file requirements</span></span>

<span data-ttu-id="f3f38-111">Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="f3f38-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="f3f38-112">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="f3f38-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="f3f38-113">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="f3f38-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="f3f38-114">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="f3f38-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="f3f38-115">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="f3f38-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="f3f38-116">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="f3f38-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="f3f38-117">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="f3f38-117">Enter only the data described below.</span></span> <span data-ttu-id="f3f38-118">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="f3f38-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="f3f38-119">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="f3f38-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="f3f38-120">**Имя столбца**</span><span class="sxs-lookup"><span data-stu-id="f3f38-120">**Column name**</span></span> | <span data-ttu-id="f3f38-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3f38-121">**Description**</span></span>  | <span data-ttu-id="f3f38-122">**Ограничения**</span><span class="sxs-lookup"><span data-stu-id="f3f38-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="f3f38-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f3f38-123">First name</span></span>  | <span data-ttu-id="f3f38-124">Имя пользователя (необязательное поле)</span><span class="sxs-lookup"><span data-stu-id="f3f38-124">User's first name (optional field)</span></span>  | <span data-ttu-id="f3f38-125">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="f3f38-125">50-character limit</span></span>  |
| <span data-ttu-id="f3f38-126">Фамилия</span><span class="sxs-lookup"><span data-stu-id="f3f38-126">Last name</span></span>  | <span data-ttu-id="f3f38-127">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="f3f38-127">User's last name (optional field)</span></span>  | <span data-ttu-id="f3f38-128">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="f3f38-128">50-character limit</span></span>  |
| <span data-ttu-id="f3f38-129">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f3f38-129">Display name</span></span>    | <span data-ttu-id="f3f38-130">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="f3f38-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="f3f38-131">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="f3f38-131">50-character limit</span></span>                         |
| <span data-ttu-id="f3f38-132">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="f3f38-132">Email</span></span>   | <span data-ttu-id="f3f38-133">Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="f3f38-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="f3f38-134">Каждый пользователь должен иметь уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f3f38-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="f3f38-135">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="f3f38-135">Status update</span></span>   | <span data-ttu-id="f3f38-136">Используется для указания того, была ли новая запись пользователя успешно создана</span><span class="sxs-lookup"><span data-stu-id="f3f38-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="f3f38-137">\*\*Оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="f3f38-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="f3f38-138">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f3f38-138">Next steps</span></span>

- [<span data-ttu-id="f3f38-139">Добавление нескольких пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="f3f38-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)