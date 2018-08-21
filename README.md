<a name='assembly'></a>
# FlowEngine.SDK

## Contents

- [Activity](#T-FlowEngine-SDK-Activity 'FlowEngine.SDK.Activity')
  - [#ctor(Id,props)](#M-FlowEngine-SDK-Activity-#ctor-System-Object,FlowEngine-SDK-interfaces-IProperties- 'FlowEngine.SDK.Activity.#ctor(System.Object,FlowEngine.SDK.interfaces.IProperties)')
  - [getId()](#M-FlowEngine-SDK-Activity-getId 'FlowEngine.SDK.Activity.getId')
  - [getProperties()](#M-FlowEngine-SDK-Activity-getProperties 'FlowEngine.SDK.Activity.getProperties')
  - [onInit()](#M-FlowEngine-SDK-Activity-onInit 'FlowEngine.SDK.Activity.onInit')
  - [run()](#M-FlowEngine-SDK-Activity-run 'FlowEngine.SDK.Activity.run')
  - [setPropertyValue(key,value)](#M-FlowEngine-SDK-Activity-setPropertyValue-System-String,System-Object- 'FlowEngine.SDK.Activity.setPropertyValue(System.String,System.Object)')
- [ActivityResult](#T-FlowEngine-SDK-ActivityResult 'FlowEngine.SDK.ActivityResult')
  - [#ctor(data,status)](#M-FlowEngine-SDK-ActivityResult-#ctor-System-Collections-Generic-IDictionary{System-String,System-Object},FlowEngine-SDK-types-ResultStatus- 'FlowEngine.SDK.ActivityResult.#ctor(System.Collections.Generic.IDictionary{System.String,System.Object},FlowEngine.SDK.types.ResultStatus)')
  - [#ctor(data,status,ex)](#M-FlowEngine-SDK-ActivityResult-#ctor-System-Collections-Generic-IDictionary{System-String,System-Object},FlowEngine-SDK-types-ResultStatus,System-Exception- 'FlowEngine.SDK.ActivityResult.#ctor(System.Collections.Generic.IDictionary{System.String,System.Object},FlowEngine.SDK.types.ResultStatus,System.Exception)')
  - [getData()](#M-FlowEngine-SDK-ActivityResult-getData 'FlowEngine.SDK.ActivityResult.getData')
  - [getException()](#M-FlowEngine-SDK-ActivityResult-getException 'FlowEngine.SDK.ActivityResult.getException')
  - [getStatus()](#M-FlowEngine-SDK-ActivityResult-getStatus 'FlowEngine.SDK.ActivityResult.getStatus')
- [IActivity](#T-FlowEngine-SDK-interfaces-IActivity 'FlowEngine.SDK.interfaces.IActivity')
- [Properties](#T-FlowEngine-SDK-Properties 'FlowEngine.SDK.Properties')
  - [addProperty(prop)](#M-FlowEngine-SDK-Properties-addProperty-FlowEngine-SDK-interfaces-IProperty- 'FlowEngine.SDK.Properties.addProperty(FlowEngine.SDK.interfaces.IProperty)')
  - [getProperty(key)](#M-FlowEngine-SDK-Properties-getProperty-System-String- 'FlowEngine.SDK.Properties.getProperty(System.String)')
- [Property](#T-FlowEngine-SDK-Property 'FlowEngine.SDK.Property')
  - [#ctor(name,value)](#M-FlowEngine-SDK-Property-#ctor-System-String,System-String- 'FlowEngine.SDK.Property.#ctor(System.String,System.String)')
  - [getName()](#M-FlowEngine-SDK-Property-getName 'FlowEngine.SDK.Property.getName')
  - [getValue()](#M-FlowEngine-SDK-Property-getValue 'FlowEngine.SDK.Property.getValue')
  - [setValue(value)](#M-FlowEngine-SDK-Property-setValue-System-Object- 'FlowEngine.SDK.Property.setValue(System.Object)')
- [ResultStatus](#T-FlowEngine-SDK-types-ResultStatus 'FlowEngine.SDK.types.ResultStatus')

<a name='T-FlowEngine-SDK-Activity'></a>
## Activity `type`

##### Namespace

FlowEngine.SDK

##### Summary

Abstract Activity class

<a name='M-FlowEngine-SDK-Activity-#ctor-System-Object,FlowEngine-SDK-interfaces-IProperties-'></a>
### #ctor(Id,props) `constructor`

##### Summary

Constructor

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| Id | [System.Object](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object 'System.Object') | Id of activity |
| props | [FlowEngine.SDK.interfaces.IProperties](#T-FlowEngine-SDK-interfaces-IProperties 'FlowEngine.SDK.interfaces.IProperties') | Properties of Activity |

<a name='M-FlowEngine-SDK-Activity-getId'></a>
### getId() `method`

##### Summary

Get Id of activity

##### Returns

id

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Activity-getProperties'></a>
### getProperties() `method`

##### Summary

Get Properties of Activity

##### Returns

IProperties

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Activity-onInit'></a>
### onInit() `method`

##### Summary

A hook that being called when initializing workflow

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Activity-run'></a>
### run() `method`

##### Summary

Run the activity

##### Returns

IResult instance

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Activity-setPropertyValue-System-String,System-Object-'></a>
### setPropertyValue(key,value) `method`

##### Summary

Set Property value

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| key | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | name of the Property |
| value | [System.Object](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object 'System.Object') | new value of the Property object |

<a name='T-FlowEngine-SDK-ActivityResult'></a>
## ActivityResult `type`

##### Namespace

FlowEngine.SDK

##### Summary

Result of Activity

<a name='M-FlowEngine-SDK-ActivityResult-#ctor-System-Collections-Generic-IDictionary{System-String,System-Object},FlowEngine-SDK-types-ResultStatus-'></a>
### #ctor(data,status) `constructor`

##### Summary

Constructor

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| data | [System.Collections.Generic.IDictionary{System.String,System.Object}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IDictionary 'System.Collections.Generic.IDictionary{System.String,System.Object}') | Data returned by the activity |
| status | [FlowEngine.SDK.types.ResultStatus](#T-FlowEngine-SDK-types-ResultStatus 'FlowEngine.SDK.types.ResultStatus') | Status |

<a name='M-FlowEngine-SDK-ActivityResult-#ctor-System-Collections-Generic-IDictionary{System-String,System-Object},FlowEngine-SDK-types-ResultStatus,System-Exception-'></a>
### #ctor(data,status,ex) `constructor`

##### Summary

Constructor

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| data | [System.Collections.Generic.IDictionary{System.String,System.Object}](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.Generic.IDictionary 'System.Collections.Generic.IDictionary{System.String,System.Object}') | Data returned by the activity |
| status | [FlowEngine.SDK.types.ResultStatus](#T-FlowEngine-SDK-types-ResultStatus 'FlowEngine.SDK.types.ResultStatus') | Status |
| ex | [System.Exception](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Exception 'System.Exception') | Exception if there is an error |

<a name='M-FlowEngine-SDK-ActivityResult-getData'></a>
### getData() `method`

##### Summary

Gets data returned by the activity

##### Returns

Data

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-ActivityResult-getException'></a>
### getException() `method`

##### Summary

Get Exception returned by the activity

##### Returns

Exception

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-ActivityResult-getStatus'></a>
### getStatus() `method`

##### Summary

Gets status returned by the activity

##### Returns

Status

##### Parameters

This method has no parameters.

<a name='T-FlowEngine-SDK-interfaces-IActivity'></a>
## IActivity `type`

##### Namespace

FlowEngine.SDK.interfaces

##### Summary

IActivity

<a name='T-FlowEngine-SDK-Properties'></a>
## Properties `type`

##### Namespace

FlowEngine.SDK

##### Summary

Contains dictionary of Property

<a name='M-FlowEngine-SDK-Properties-addProperty-FlowEngine-SDK-interfaces-IProperty-'></a>
### addProperty(prop) `method`

##### Summary

Add Property object

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| prop | [FlowEngine.SDK.interfaces.IProperty](#T-FlowEngine-SDK-interfaces-IProperty 'FlowEngine.SDK.interfaces.IProperty') | property object |

<a name='M-FlowEngine-SDK-Properties-getProperty-System-String-'></a>
### getProperty(key) `method`

##### Summary

Get Property object

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| key | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | the name of object |

<a name='T-FlowEngine-SDK-Property'></a>
## Property `type`

##### Namespace

FlowEngine.SDK

##### Summary

Property definition used by Properties injected in Activity

<a name='M-FlowEngine-SDK-Property-#ctor-System-String,System-String-'></a>
### #ctor(name,value) `constructor`

##### Summary

Property Constructor

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| name | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | Name of Property |
| value | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | Value of Property |

<a name='M-FlowEngine-SDK-Property-getName'></a>
### getName() `method`

##### Summary

Returns name of Property

##### Returns

returns name

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Property-getValue'></a>
### getValue() `method`

##### Summary

Returns value of Property

##### Returns

returns value

##### Parameters

This method has no parameters.

<a name='M-FlowEngine-SDK-Property-setValue-System-Object-'></a>
### setValue(value) `method`

##### Summary

Set value of a Property

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| value | [System.Object](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object 'System.Object') | property value |

<a name='T-FlowEngine-SDK-types-ResultStatus'></a>
## ResultStatus `type`

##### Namespace

FlowEngine.SDK.types

##### Summary

ResultStatus

