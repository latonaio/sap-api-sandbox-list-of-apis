<p align="center"> <img src="https://user-images.githubusercontent.com/91356865/144049159-1ebbd095-87d2-4a3c-81cb-277cc1d4c7b7.png" width="300"> </p> <p align="center"> Starting Up the API Environment on a "Full-of-Beans" SandBox </p>

***

# sap-sandbox-list-of-apis  
sap-sandbox-list-of-apis は、sap-sandbox で 整備された SAP APIs（及び対応する 各 APIサービスランタイム の package responses） をまとめたリポジトリです。  
sap-sandbox-list-of-apis の 「sandbox」は、Netflix 韓国ドラマ 「START-UP」 より、すべての開発者のための 地ならし になればという想いから命名されました。  
なお、各リソースは、そのままクラウド環境におけるアプリケーションにも適用可能です。  

## 前提条件  
sap-sandbox-list-of-apis は、オンプレミス版である（＝クラウド版ではない）SAPS4HANA API の利用を前提としています。  
クラウド版APIを利用する場合は、ご注意ください。  

## Central Functions ##

### Business Partner ###

* A_BusinessPartner / [general.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/general.go)
* A_BusinessPartnerRole / [role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/role.go)
* A_BusinessPartnerAddress / [address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/address.go)
* A_BusinessPartnerBank / [bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/bank.go)
* ToRole / [to_role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_role.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_address.go)
* ToBank / [to_bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads/blob/main/SAP_API_Caller/responses/to_bank.go)

## Logistics ##

### Product Master ###

* A_Product / [general.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/general.go)
* A_ProductPlant / [plant.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/plant.go)
* A_ProductPlantSales / [sales_plant.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/sales_plant.go)
* A_ProductPlantProcurement / [procurement.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/procurement.go)
* A_ProductPlantMRPArea / [mrp_area.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/mrp_area.go)
* A_ProductWorkScheduling / [work_scheduling.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/work_scheduling.go)
* A_ProductSalesDelivery / [sales_organization.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/sales_organization.go)
* A_ProductValuationAccount / [accounting.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/accounting.go)
* A_ProductDescription / [product_desc.go](https://github.com/latonaio/sap-api-integrations-product-master-reads/blob/main/SAP_API_Caller/responses/product_desc.go)

### Batch Master Record ###
* Batch / [batch.go](https://github.com/latonaio/sap-api-integrations-batch-master-record-reads/blob/main/SAP_API_Caller/responses/batch.go)

## Inventory Management ##

### Material Stock ###

* A_MatlStkInAcctMod / [material_stock.go](https://github.com/latonaio/sap-api-integrations-material-stock-reads/blob/main/SAP_API_Caller/responses/material_stock.go)
* ToMaterialStock / [to_material_stock.go](https://github.com/latonaio/sap-api-integrations-material-stock-reads/blob/main/SAP_API_Caller/responses/to_material_stock.go)

### Reservation Document ###

* A_ReservationDocumentHeader / [header.go](https://github.com/latonaio/sap-api-integrations-reservation-document-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_ReservationDocumentItem / [item.go](https://github.com/latonaio/sap-api-integrations-reservation-document-reads/blob/main/SAP_API_Caller/responses/item.go)

### Inbound Delivery ###
* A_InbDeliveryHeader / [header.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/header.go)
* ToPartner / [to_partner.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_partner.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_address.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-inbound-delivery-reads/blob/main/SAP_API_Caller/responses/to_item.go)

### Material Document ###

* A_MaterialDocumentHeader / [header.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_MaterialDocumentHeaderItem / [item.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-material-document-reads/blob/main/SAP_API_Caller/responses/to_item.go)

### Customer Master ###

* A_BusinessPartner / [general.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/general.go)
* A_BusinessPartnerRole / [role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/role.go)
* A_BusinessPartnerAddress / [address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/address.go)
* A_BusinessPartnerBank / [bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/bank.go)
* A_Customer / [customer.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/customer.go)
* A_CustomerSalesArea / [sales_area.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/sales_area.go)
* A_CustomerCompany / [company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/company.go)
* ToRole / [to_role.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_role.go)
* ToAddress / [to_address.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_address.go)
* ToBank / [to_bank.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_bank.go)
* ToCustomer / [to_customer.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_customer.go)
* ToSalesArea / [to_sales_area.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_sales_area.go)
* ToPartnerFunction / [to_partner_function.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_partner_function.go)
* ToCompany / [to_company.go](https://github.com/latonaio/sap-api-integrations-business-partner-reads-customer/blob/main/SAP_API_Caller/responses/to_company.go)

### Sales Pricing ###

* A_SlsPrcgCndnRecdValidity / [pricing_condition_validity.go](https://github.com/latonaio/sap-api-integrations-sales-pricing-reads/blob/main/SAP_API_Caller/responses/pricing_condition_validity.go)
* ToConditionRecord / [to_condition_record.go](https://github.com/latonaio/sap-api-integrations-sales-pricing-reads/blob/main/SAP_API_Caller/responses/to_condition_record.go)

### Sales Inquiry ###
* A_SalesInquiry / [header.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesInquiryItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-inquiry-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)

### Sales Quotation ###
* A_SalesQuotation / [header.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/header.go)
* A_SalesQuotationItem / [item.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/item.go)
* ToHeaderPartner / [to_header_partner.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_header_partner.go)
* ToItem / [to_item.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_item.go)
* ToItemPricingElement / [to_item_pricing_element.go](https://github.com/latonaio/sap-api-integrations-sales-quotation-reads/blob/main/SAP_API_Caller/responses/to_item_pricing_element.go)
