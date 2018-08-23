---
title: "[WebUI] Verify Option Not Selected By Value" 
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/webui-verify-option-not-selected-by-value.html 
description: 
---
Description

Verify if the options with the given value are not selected.

![](../../images/katalon-studio/docs/webui-verify-option-not-selected-by-value/image2017-3-1 18_20_51.png)

Parameters
----------

| Param | Param Type | Mandatory | Description |
| --- | --- | --- | --- |
| to | TestObject | Required | Represent a web element. |
| value | String | Required | Value of the options to be verified if not being selected. |
| isRegex | boolean | Required | True if the label is a regular expression, false by default. |
| timeout | int | Required | System will wait at most timeout (seconds) to return the result. |
| flowControl | FailureHandling | Optional | Specify [failure handling](https://docs.katalon.com/x/qAAM) schema to determine whether the execution should be allowed to continue or stop |

Returns
-------

| Param Type | Description |
| --- | --- |
| boolean | 
*   **true:** if all options with given value are NOT selected.
*   **false: **if all options with given value are selected

 |

Example
-------

You want to verify if an item with value 'HongKong Cura Health Center' does not exist in the list.

```
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint
import com.kms.katalon.core.checkpoint.CheckpointFactory as CheckpointFactory
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as MobileBuiltInKeywords
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testcase.TestCaseFactory as TestCaseFactory
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testdata.TestDataFactory as TestDataFactory
import com.kms.katalon.core.testobject.ObjectRepository as ObjectRepository
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WSBuiltInKeywords
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUiBuiltInKeywords
import internal.GlobalVariable as GlobalVariable
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS

'Open browser and navigate to demo AUT site.'
WebUI.openBrowser(GlobalVariable.G_SiteURL)

'Click on \'Book Appointment\' button'
WebUI.click(findTestObject('Page_CuraHomepage/btn_MakeAppointment'))

'Verify \'HongKong Cura Health Center\' option in \'Facility\' list is not selected'
WebUI.verifyOptionNotSelectedByValue(findTestObject('Page_CuraAppointment/lst_Facility'), 'HongKong Cura Health Center', 
    false, 20)

'Close browser'
WebUI.closeBrowser()
```