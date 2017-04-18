---
title: "분석 추적 이벤트 참조 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "분석 추적 [WCF]. 참조"
ms.assetid: e44540cf-44a1-4efc-b965-7fbfd2131d73
caps.latest.revision: 50
author: "Erikre"
ms.author: "erikre"
manager: "erikre"
caps.handback.revision: 50
---
# 분석 추적 이벤트 참조
다음 표에서는 [!INCLUDE[indigo2](../../../../../includes/indigo2-md.md)] 분석 추적과 연결된 이벤트 수준, ID 및 메시지를 정의합니다.  
  
## 이벤트 참조  
  
|이벤트 ID|이벤트 수준|이벤트 메시지|키워드|  
|------------|------------|-------------|---------|  
|[131 \- BufferPoolAllocation](../../../../../docs/framework/wcf/diagnostics/etw/131-bufferpoolallocation.md)|Verbose|풀에서 %1바이트를 할당하는 중입니다.|인프라|  
|[132 \- BufferPoolChangeQuota](../../../../../docs/framework/wcf/diagnostics/etw/132-bufferpoolchangequota.md)|Verbose|크기가 %1인 BufferPool의 할당량을 %2\(으\)로 변경하는 중입니다.|인프라|  
|[133 \- ActionItemScheduled](../../../../../docs/framework/wcf/diagnostics/etw/133-actionitemscheduled.md)|Verbose|IO 스레드 스케줄러 콜백이 호출되었습니다.|인프라|  
|[134 \- ActionItemCallbackInvoked](../../../../../docs/framework/wcf/diagnostics/etw/134-actionitemcallbackinvoked.md)|Verbose|IO 스레드 스케줄러 콜백이 호출되었습니다.|인프라|  
|[201 \- ClientMessageInspectorAfterReceiveInvoked](../../../../../docs/framework/wcf/diagnostics/etw/201-clientmessageinspectorafterreceiveinvoked.md)|정보|디스패처가 '%1' 형식의 ClientMessageInspector에 대해 'AfterReceiveReply'를 호출했습니다.|문제 해결, ServiceModel|  
|[202 \- ClientMessageInspectorBeforeSendInvoked](../../../../../docs/framework/wcf/diagnostics/etw/202-clientmessageinspectorbeforesendinvoked.md)|정보|디스패처가 '%1' 형식의 ClientMessageInspector에 대해 'BeforeSendRequest'를 호출했습니다.|문제 해결, ServiceModel|  
|[203 \- ClientParameterInspectorAfterCallInvoked](../../../../../docs/framework/wcf/diagnostics/etw/203-clientparameterinspectoraftercallinvoked.md)|정보|디스패처가 '%1' 형식의 ClientParameterInspector에 대해 'AfterCall'을  호출했습니다.|문제 해결, ServiceModel|  
|[204 \- ClientParameterInspectorBeforeCallInvoked](../../../../../docs/framework/wcf/diagnostics/etw/204-clientparameterinspectorbeforecallinvoked.md)|정보|디스패처가 '%1' 형식의 ClientParameterInspector에 대해 'BeforeCall'을 호출했습니다.|문제 해결, ServiceModel|  
|[205 \- OperationInvoked](../../../../../docs/framework/wcf/diagnostics/etw/205-operationinvoked.md)|정보|OperationInvoker가 '%1' 메서드를 호출했습니다.|EndToEndMonitoring, 문제 해결, ServiceModel|  
|[206 \- ErrorHandlerInvoked](../../../../../docs/framework/wcf/diagnostics/etw/206-errorhandlerinvoked.md)|정보|디스패처가 '%3' 형식의 예외와 함께 '%1' 형식의 ErrorHandler를 호출했습니다.  ErrorHandled \=\= '%2'.|문제 해결, ServiceModel|  
|[207 \- FaultProviderInvoked](../../../../../docs/framework/wcf/diagnostics/etw/207-faultproviderinvoked.md)|정보|디스패처가 '%2' 형식의 예외와 함께 '%1' 형식의 FaultProvider를 호출했습니다.|문제 해결, ServiceModel|  
|[208 \- MessageInspectorAfterReceiveInvoked](../../../../../docs/framework/wcf/diagnostics/etw/208-messageinspectorafterreceiveinvoked.md)|정보|디스패처가 '%1' 형식의 MessageInspector에 대해 'AfterReceiveReply'를 호출했습니다.|문제 해결, ServiceModel|  
|[209 \- MessageInspectorBeforeSendInvoked](../../../../../docs/framework/wcf/diagnostics/etw/209-messageinspectorbeforesendinvoked.md)|정보|디스패처가 '%1' 형식의 MessageInspector에 대해 'BeforeSendRequest'를 호출했습니다.|문제 해결, ServiceModel|  
|[210 \- MessageThrottleExceeded](../../../../../docs/framework/wcf/diagnostics/etw/210-messagethrottleexceeded.md)|경고|'%1'의 스로틀 한계 '%2'에 도달했습니다.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[211 \- ParameterInspectorAfterCallInvoked](../../../../../docs/framework/wcf/diagnostics/etw/211-parameterinspectoraftercallinvoked.md)|정보|디스패처가 '%1' 형식의 ParameterInspector에 대해 'AfterCall'을 호출했습니다.|문제 해결, ServiceModel|  
|[212 \- ParameterInspectorBeforeCallInvoked](../../../../../docs/framework/wcf/diagnostics/etw/212-parameterinspectorbeforecallinvoked.md)|정보|디스패처가 '%1' 형식의 ParameterInspector에 대해 'BeforeCall'을 호출했습니다.|문제 해결, ServiceModel|  
|[213 \- ServiceHostStarted](../../../../../docs/framework/wcf/diagnostics/etw/213-servicehoststarted.md)|LogAlways|ServiceHost 시작: '%1'.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[214 \- OperationCompleted](../../../../../docs/framework/wcf/diagnostics/etw/214-operationcompleted.md)|정보|OperationInvoker가 '%1' 메서드에 대한 호출을 완료했습니다.  메서드 호출 기간은 '%2'밀리초입니다.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[215 \- MessageReceivedByTransport](../../../../../docs/framework/wcf/diagnostics/etw/215-messagereceivedbytransport.md)|정보|전송이 '%1'에서 메시지를 받았습니다.|문제 해결, ServiceModel|  
|[216 \- MessageSentByTransport](../../../../../docs/framework/wcf/diagnostics/etw/216-messagesentbytransport.md)|정보|전송이 '%1'에 메시지를 보냈습니다.|문제 해결, ServiceModel|  
|[217 \- ClientOperationPrepared](../../../../../docs/framework/wcf/diagnostics/etw/217-clientoperationprepared.md)|정보|클라이언트가 '%2' 계약에 정의된 '%1' 작업을 실행하는 중입니다.  메시지를 '%3'\(으\)로 보냅니다.|문제 해결, ServiceModel|  
|[218 \- ClientOperationCompleted](../../../../../docs/framework/wcf/diagnostics/etw/218-clientoperationcompleted.md)|정보|클라이언트가 '%2' 계약에 정의된 '%1' 작업 실행을 완료했습니다.  메시지가 '%3'\(으\)로 전송되었습니다.|문제 해결, ServiceModel|  
|[219 \- ServiceException](../../../../../docs/framework/wcf/diagnostics/etw/219-serviceexception.md)|오류|메시지를 처리하는 동안 '%2' 형식의 처리되지 않은 예외가 발생했습니다.  전체 예외 ToString: %1.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[220 \- MessageSentToTransport](../../../../../docs/framework/wcf/diagnostics/etw/220-messagesenttotransport.md)|정보|디스패처가 전송에 메시지를 보냈습니다.  Correlation ID \=\= '%1'.|EndToEndMonitoring, 문제 해결, ServiceModel|  
|[221 \- MessageReceivedFromTransport](../../../../../docs/framework/wcf/diagnostics/etw/221-messagereceivedfromtransport.md)|정보|디스패처가 전송에서 메시지를 받았습니다.  Correlation ID \=\= '%1'.|EndToEndMonitoring, 문제 해결, ServiceModel|  
|[222 \- OperationFailed](../../../../../docs/framework/wcf/diagnostics/etw/222-operationfailed.md)|경고|OperationInvoker의 호출을 받은 '%1' 메서드에서 처리되지 않은 예외가 발생했습니다.  메서드 호출 기간은 '%2'밀리초입니다.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[223 \- OperationFaulted](../../../../../docs/framework/wcf/diagnostics/etw/223-operationfaulted.md)|경고|OperationInvoker의 호출을 받은 '%1' 메서드에서 FaultException이 발생했습니다.  메서드 호출 기간은 '%2'밀리초입니다.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[224 \- MessageThrottleAtSeventyPercent](../../../../../docs/framework/wcf/diagnostics/etw/224-messagethrottleatseventypercent.md)|경고|'%2'의 스로틀 제한 '%1'이\(가\) 70퍼센트입니다.|HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[226 \- IdleServicesClosed](../../../../../docs/framework/wcf/diagnostics/etw/226-idleservicesclosed.md)|LogAlways|활성화된 총 %2개 서비스 중에서 %1개의 유휴 서비스가 종료되었습니다.|HealthMonitoring WebHost|  
|[301 \- UserDefinedErrorOccurred](../../../../../docs/framework/wcf/diagnostics/etw/301-userdefinederroroccurred.md)|오류|이름: '%1', 참조: '%2', 페이로드: %3.|UserEvents, HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[302 \- UserDefinedWarningOccurred](../../../../../docs/framework/wcf/diagnostics/etw/302-userdefinedwarningoccurred.md)|경고|이름: '%1', 참조: '%2', 페이로드: %3.|UserEvents, HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[303 \- UserDefinedInformationEventOccured](../../../../../docs/framework/wcf/diagnostics/etw/303-userdefinedinformationeventoccured.md)|정보|이름: '%1', 참조: '%2', 페이로드: %3.|UserEvents, HealthMonitoring, EndToEndMonitoring, 문제 해결, ServiceModel|  
|[401\- StopSignPostEvent](../../../../../docs/framework/wcf/diagnostics/etw/401-stopsignpostevent.md)|정보|동작 경계입니다.|문제 해결|  
|[402 \- StartSignpostEvent](../../../../../docs/framework/wcf/diagnostics/etw/402-startsignpostevent.md)|정보|동작 경계입니다.|문제 해결|  
|[403 \- SuspendSignpostEvent](../../../../../docs/framework/wcf/diagnostics/etw/403-suspendsignpostevent.md)|정보|동작 경계입니다.|문제 해결|  
|[404 \- ResumeSignpostEvent](../../../../../docs/framework/wcf/diagnostics/etw/404-resumesignpostevent.md)|정보|동작 경계입니다.|문제 해결|  
|[451 \- MessageLogInfo](../../../../../docs/framework/wcf/diagnostics/etw/451-messageloginfo.md)|정보|%1|문제 해결, WCFMessageLogging|  
|[452 \- MessageLogWarning](../../../../../docs/framework/wcf/diagnostics/etw/452-messagelogwarning.md)|경고|%1|문제 해결, WCFMessageLogging|  
|[499 \- TransferEmitted](../../../../../docs/framework/wcf/diagnostics/etw/499-transferemitted.md)|LogAlways|전송 이벤트를 내보냈습니다.|문제 해결, UserEvents, EndToEndMonitoring, ServiceModel, WFTracking, ServiceHost, WCFMessageLogging|  
|[501 \- CompilationStart](../../../../../docs/framework/wcf/diagnostics/etw/501-compilationstart.md)|정보|컴파일을 시작합니다.|WebHost|  
|[502 \- CompilationStop](../../../../../docs/framework/wcf/diagnostics/etw/502-compilationstop.md)|정보|컴파일을 종료합니다.|WebHost|  
|[503 \- ServiceHostFactoryCreationStart](../../../../../docs/framework/wcf/diagnostics/etw/503-servicehostfactorycreationstart.md)|정보|ServiceHostFactory 만들기를 시작합니다.|WebHost|  
|[504 \- ServiceHostFactoryCreationStop](../../../../../docs/framework/wcf/diagnostics/etw/504-servicehostfactorycreationstop.md)|정보|ServiceHostFactory 만들기를 종료합니다.|WebHost|  
|[505 \- CreateServiceHostStart](../../../../../docs/framework/wcf/diagnostics/etw/505-createservicehoststart.md)|정보|CreateServiceHost를 시작합니다.|WebHost|  
|[506 \- CreateServiceHostStop](../../../../../docs/framework/wcf/diagnostics/etw/506-createservicehoststop.md)|정보|CreateServiceHost를 종료합니다.|WebHost|  
|[507 \- HostedTransportConfigurationManagerConfigInitStart](../../../../../docs/framework/wcf/diagnostics/etw/507-hostedtransportconfigurationmanagerconfiginitstart.md)|정보|HostedTransportConfigurationManager에서 구성 초기화를 시작합니다.|WebHost|  
|[508 \- HostedTransportConfigurationManagerConfigInitStop](../../../../../docs/framework/wcf/diagnostics/etw/508-hostedtransportconfigurationmanagerconfiginitstop.md)|정보|HostedTransportConfigurationManager에서 구성 초기화를 종료합니다.|WebHost|  
|[509 \- ServiceHostOpenStart](../../../../../docs/framework/wcf/diagnostics/etw/509-servicehostopenstart.md)|정보|HostedTransportConfigurationManager에서 구성 초기화를 종료합니다.|ServiceHost|  
|[510 \- ServiceHostOpenStop](../../../../../docs/framework/wcf/diagnostics/etw/510-servicehostopenstop.md)|정보|ServiceHost 열기가 완료되었습니다.|ServiceHost|  
|[513 \- WebHostRequestStart](../../../../../docs/framework/wcf/diagnostics/etw/513-webhostrequeststart.md)|정보|AppDomain '%1'에서 가상 경로가 '%2'인 요청을 수신했습니다.|WebHost|  
|[514 \- WebHostRequestStop](../../../../../docs/framework/wcf/diagnostics/etw/514-webhostrequeststop.md)|정보|WebHostRequest가 중지됩니다.|WebHost|  
|[601 \- CBAEntryRead](../../../../../docs/framework/wcf/diagnostics/etw/601-cbaentryread.md)|Verbose|처리한 ServiceActivation 요소 상대 주소: '%1', 정규화된 상대 주소 '%2'||  
|[602 \- CBAMatchFound](../../../../../docs/framework/wcf/diagnostics/etw/602-cbamatchfound.md)|Verbose|들어오는 요청이 주소가 '%1'인 ServiceActivation 요소와 일치합니다.||  
|[603 \- AspNetRoutingService](../../../../../docs/framework/wcf/diagnostics/etw/603-aspnetroutingservice.md)|Verbose|들어오는 요청이 주소가 %1인 Asp.Net 경로에 정의된 WCF 서비스와 일치합니다.|RoutingServices|  
|[604 \- AspNetRoute](../../../../../docs/framework/wcf/diagnostics/etw/604-aspnetroute.md)|Verbose|serviceType이 '%2'이고 serviceHostFactoryType이 '%3'인 새 Asp.Net 경로 '%1'이\(가\) 추가되었습니다.|RoutingServices|  
|[605 \- IncrementBusyCount](../../../../../docs/framework/wcf/diagnostics/etw/605-incrementbusycount.md)|Verbose|IncrementBusyCount를 호출했습니다.  원본: %1|WebHost|  
|[606 \- DecrementBusyCount](../../../../../docs/framework/wcf/diagnostics/etw/606-decrementbusycount.md)|Verbose|DecrementBusyCount를 호출했습니다.  원본: %1|WebHost|  
|[701 \- ServiceChannelOpenStart](../../../../../docs/framework/wcf/diagnostics/etw/701-servicechannelopenstart.md)|Verbose|ServiceChannelOpen이 시작되었습니다.|WebHost|  
|[702 \- ServiceChannelOpenStop](../../../../../docs/framework/wcf/diagnostics/etw/702-servicechannelopenstop.md)|정보|ServiceChannelOpen이 완료되었습니다.|ServiceModel|  
|[703 \- ServiceChannelCallStart](../../../../../docs/framework/wcf/diagnostics/etw/703-servicechannelcallstart.md)|정보|ServiceChannelCall이 시작되었습니다.|ServiceModel|  
|[704 \- ServiceChannelBeginCallStart](../../../../../docs/framework/wcf/diagnostics/etw/704-servicechannelbegincallstart.md)|정보|ServiceChannel 비동기 호출이 시작되었습니다.|ServiceModel|  
|[706 \- HttpSendMessageStart](../../../../../docs/framework/wcf/diagnostics/etw/706-httpsendmessagestart.md)|Verbose|Http 전송 요청이 시작됩니다.|HTTP|  
|[707 \- HttpSendStop](../../../../../docs/framework/wcf/diagnostics/etw/707-httpsendstop.md)|Verbose|Http 전송 요청이 중지됩니다.|HTTP|  
|[708 \- HttpMessageReceiveStart](../../../../../docs/framework/wcf/diagnostics/etw/708-httpmessagereceivestart.md)|Verbose|http 전송으로부터 메시지가 수신되었습니다.|HTTP|  
|[709 \- DispatchMessageStart](../../../../../docs/framework/wcf/diagnostics/etw/709-dispatchmessagestart.md)|정보|메시지 디스패치가 시작되었습니다.|ServiceModel|  
|[710 \- HttpContextBeforeProcessAuthentication](../../../../../docs/framework/wcf/diagnostics/etw/710-httpcontextbeforeprocessauthentication.md)|Verbose|메시지 디스패치를 위한 인증을 시작합니다.|ServiceModel|  
|[711 \- DispatchMessageBeforeAuthorization](../../../../../docs/framework/wcf/diagnostics/etw/711-dispatchmessagebeforeauthorization.md)|Verbose|메시지 디스패치를 위한 권한 부여를 시작합니다.|ServiceModel|  
|[712 \- DispatchMessageStop](../../../../../docs/framework/wcf/diagnostics/etw/712-dispatchmessagestop.md)|정보|메시지 디스패치가 완료되었습니다.|ServiceModel|  
|[715 \- ClientChannelOpenStart](../../../../../docs/framework/wcf/diagnostics/etw/715-clientchannelopenstart.md)|정보|ServiceChannel 열기가 시작됩니다.|ServiceModel|  
|[716 \- ClientChannelOpenStop](../../../../../docs/framework/wcf/diagnostics/etw/716-clientchannelopenstop.md)|정보|ServiceChannel 열기가 중지됩니다.|ServiceModel|  
|[717 \- HttpSendStreamedMessageStart](../../../../../docs/framework/wcf/diagnostics/etw/717-httpsendstreamedmessagestart.md)|정보|Http 전송 스트리밍 메시지가 시작되었습니다.|HTTP|  
|[1400 \- ChannelInitializationTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1400-channelinitializationtimeout.md)|오류|1%|ServiceModel|  
|[1401 \- CloseTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1401-closetimeout.md)|오류|1%|ServiceModel|  
|[1402 \- IdleTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1402-idletimeout.md)|오류|%1 연결 풀 키: %2|ServiceModel|  
|[1403 \- LeaseTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1403-leasetimeout.md)|정보|%1 연결 풀 키: %2|ServiceModel|  
|[1405 \- OpenTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1405-opentimeout.md)|오류|%1|ServiceModel|  
|[1406 \- ReceiveTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1406-receivetimeout.md)|오류|%1|ServiceModel|  
|[1407 \- SendTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1407-sendtimeout.md)|오류|%1|ServiceModel|  
|[1409 \- InactivityTimeout](../../../../../docs/framework/wcf/diagnostics/etw/1409-inactivitytimeout.md)|정보|%1|ServiceModel|  
|[1416 \- MaxReceivedMessageSizeExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1416-maxreceivedmessagesizeexceeded.md)|오류|%1|할당량|  
|[1417 \- MaxSentMessageSizeExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1417-maxsentmessagesizeexceeded.md)|오류|%1|할당량|  
|[1418 \- MaxOutboundConnectionsPerEndpointExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1418-maxoutboundconnectionsperendpointexceeded.md)|정보|%1|할당량|  
|[1419 \- MaxPendingConnectionsExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1419-maxpendingconnectionsexceeded.md)|정보|%1|할당량|  
|[1420 \- ReaderQuotaExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1420-readerquotaexceeded.md)|오류|%1|할당량|  
|[1422 \- NegotiateTokenAuthenticatorStateCacheExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1422-negotiatetokenauthenticatorstatecacheexceeded.md)|오류|%1|할당량|  
|[1423 \- NegotiateTokenAuthenticatorStateCacheRatio](../../../../../docs/framework/wcf/diagnostics/etw/1423-negotiatetokenauthenticatorstatecacheratio.md)|Verbose|협상 토큰 인증자 상태 캐시 비율: %1\/%2|할당량|  
|[1424 \- SecuritySessionRatio](../../../../../docs/framework/wcf/diagnostics/etw/1424-securitysessionratio.md)|Verbose|보안 세션 비율: %1\/%2|할당량|  
|[1430 \- PendingConnectionsRatio](../../../../../docs/framework/wcf/diagnostics/etw/1430-pendingconnectionsratio.md)|Verbose|보류 중인 연결 비율: %1\/%2|할당량|  
|[1431 \- ConcurrentCallsRatio](../../../../../docs/framework/wcf/diagnostics/etw/1431-concurrentcallsratio.md)|Verbose|동시 세션 비율: %1\/%2|할당량|  
|[1432 \- ConcurrentSessionsRatio](../../../../../docs/framework/wcf/diagnostics/etw/1432-concurrentsessionsratio.md)|Verbose|동시 세션 비율: %1\/%2|할당량|  
|[1433 \- OutboundConnectionsPerEndpointRatio](../../../../../docs/framework/wcf/diagnostics/etw/1433-outboundconnectionsperendpointratio.md)|Verbose|끝점당 아웃바운드 연결 비율: %1\/%2|할당량|  
|[1433 \- OutboundConnectionsPerEndpointRatio](../../../../../docs/framework/wcf/diagnostics/etw/1433-outboundconnectionsperendpointratio.md)|Verbose|끝점당 아웃바운드 연결 비율: %1\/%2|할당량|  
|[1436 \- PendingMessagesPerChannelRatio](../../../../../docs/framework/wcf/diagnostics/etw/1436-pendingmessagesperchannelratio.md)|Verbose|채널당 보류 중인 메시지 비율: %1\/%2|할당량|  
|[1438 \- ConcurrentInstancesRatio](../../../../../docs/framework/wcf/diagnostics/etw/1438-concurrentinstancesratio.md)|Verbose|동시 인스턴스 비율: %1\/%2|할당량|  
|[1439 \- PendingAcceptsAtZero](../../../../../docs/framework/wcf/diagnostics/etw/1439-pendingacceptsatzero.md)|정보|보류 중인 수락 항목 없음|할당량|  
|[1441 \- MaxSessionSizeReached](../../../../../docs/framework/wcf/diagnostics/etw/1441-maxsessionsizereached.md)|경고|1%|할당량|  
|[1442 \- ReceiveRetryCountReached](../../../../../docs/framework/wcf/diagnostics/etw/1442-receiveretrycountreached.md)|경고|ID가 '%1'인 MSMQ 메시지에서 수신 재시도 횟수에 도달했습니다.|할당량|  
|[1443 \- MaxRetryCyclesExceededMsmq](../../../../../docs/framework/wcf/diagnostics/etw/1443-maxretrycyclesexceededmsmq.md)|오류|ID가 '%1'인 MSMQ 메시지에서 최대 재시도 주기가 초과되었습니다.|할당량|  
|[1445 \- ReadPoolMiss](../../../../../docs/framework/wcf/diagnostics/etw/1445-readpoolmiss.md)|Verbose|새 '%1'이\(가\) 만들어졌습니다.|할당량|  
|[1446 \- WritePoolMiss](../../../../../docs/framework/wcf/diagnostics/etw/1446-writepoolmiss.md)|Verbose|새 '%1'이\(가\) 만들어졌습니다.|할당량|  
|[1451 \- MaxRetryCyclesExceeded](../../../../../docs/framework/wcf/diagnostics/etw/1451-maxretrycyclesexceeded.md)|오류|1%|할당량|  
|[3300 \- ReceiveContextCompleteFailed](../../../../../docs/framework/wcf/diagnostics/etw/3300-receivecontextcompletefailed.md)|경고|'%1'을\(를\) 완료하지 못했습니다.|채널|  
|[3301 \- ReceiveContextAbandonFailed](../../../../../docs/framework/wcf/diagnostics/etw/3301-receivecontextabandonfailed.md)|경고|%1을\(를\) 중단하지 못했습니다.|채널|  
|[3303 \- ReceiveContextAbandonWithException](../../../../../docs/framework/wcf/diagnostics/etw/3303-receivecontextabandonwithexception.md)|경고|컨텍스트 수신 오류가 발생했습니다.|ServiceModel|  
|[3303 \- ReceiveContextAbandonWithException](../../../../../docs/framework/wcf/diagnostics/etw/3303-receivecontextabandonwithexception.md)|정보|%1이\(가\) %2 예외와 함께 중단되었습니다.|채널|  
|[3305 \- ClientBaseCachedChannelFactoryCount](../../../../../docs/framework/wcf/diagnostics/etw/3305-clientbasecachedchannelfactorycount.md)|정보|캐시된 채널 팩터리 수: '%1'. 최대 '%2'개의 채널 팩터리를 캐시할 수 있습니다.|ServiceModel|  
|[3306 \- ClientBaseChannelFactoryAgedOutofCache](../../../../../docs/framework/wcf/diagnostics/etw/3306-clientbasechannelfactoryagedoutofcache.md)|정보|캐시가 해당 한도 '%1'에 도달했기 때문에 채널 팩터리가 캐시에서 만료되었습니다.|ServiceModel|  
|[3307 \- ClientBaseChannelFactoryCacheHit](../../../../../docs/framework/wcf/diagnostics/etw/3307-clientbasechannelfactorycachehit.md)|정보|캐시에서 사용된 일치하는 채널 팩터리가 발견되었습니다.|ServiceModel|  
|[3308 \- ClientBaseUsingLocalChannelFactory](../../../../../docs/framework/wcf/diagnostics/etw/3308-clientbaseusinglocalchannelfactory.md)|정보|캐시에서 채널 팩터리를 사용하는 중이 아닙니다.  즉 인스턴스에 대해 캐싱이 해제되었습니다.|ServiceModel|  
|[3309 \- QueryCompositionExecuted](../../../../../docs/framework/wcf/diagnostics/etw/3309-querycompositionexecuted.md)|정보|'%1'을\(를\) 사용한 쿼리 작성이 요청 Uri: '%2'에서 실행되었습니다.|ServiceModel|  
|[3310 \- DispatchFailed](../../../../../docs/framework/wcf/diagnostics/etw/3310-dispatchfailed.md)|오류|'%1' 작업이 디스패치되었지만 오류가 발생했습니다.|ServiceModel|  
|[3311 \- DispatchSuccessful](../../../../../docs/framework/wcf/diagnostics/etw/3311-dispatchsuccessful.md)|정보|'%1' 작업이 성공적으로 디스패치되었습니다.|ServiceModel|  
|[3312 \- MessageReadByEncoder](../../../../../docs/framework/wcf/diagnostics/etw/3312-messagereadbyencoder.md)|정보|인코더가 크기가 '%1'바이트인 메시지를 읽었습니다.|채널|  
|[3312 \- MessageReadByEncoder](../../../../../docs/framework/wcf/diagnostics/etw/3312-messagereadbyencoder.md)|정보|인코더가 크기가 '%1'바이트인 메시지를 썼습니다.|채널|  
|[3314 \- SessionIdleTimeout](../../../../../docs/framework/wcf/diagnostics/etw/3314-sessionidletimeout.md)|오류|URI: '%1'에 대한 유휴 채널에 대해 세션을 중단하는 중입니다.|ServiceModel|  
|[3319 \- SocketAcceptEnqueued](../../../../../docs/framework/wcf/diagnostics/etw/3319-socketacceptenqueued.md)|Verbose|연결 수락이 시작되었습니다.|TCP|  
|[3320 \- SocketAccepted](../../../../../docs/framework/wcf/diagnostics/etw/3320-socketaccepted.md)|Verbose|ListenerId:%1에서 SocketId:%2이\(가\) 수락되었습니다.|TCP|  
|[3321 \- ConnectionPoolMiss](../../../../../docs/framework/wcf/diagnostics/etw/3321-connectionpoolmiss.md)|Verbose|%1에 대한 풀에 사용 가능한 연결이 없고 %2개의 연결을 사용 중입니다.|채널|  
|[3322 \- DispatchFormatterDeserializeRequestStart](../../../../../docs/framework/wcf/diagnostics/etw/3322-dispatchformatterdeserializerequeststart.md)|Verbose|디스패처가 요청 메시지의 역직렬화를 시작했습니다.|ServiceModel|  
|[3323 \- DispatchFormatterDeserializeRequestStop](../../../../../docs/framework/wcf/diagnostics/etw/3323-dispatchformatterdeserializerequeststop.md)|Verbose|디스패처가 요청 메시지의 역직렬화를 완료했습니다.|ServiceModel|  
|[3324 \- DispatchFormatterSerializeReplyStart](../../../../../docs/framework/wcf/diagnostics/etw/3324-dispatchformatterserializereplystart.md)|Verbose|디스패처가 회신 메시지의 직렬화를 시작했습니다.|ServiceModel|  
|[3325 \- DispatchFormatterSerializeReplyStop](../../../../../docs/framework/wcf/diagnostics/etw/3325-dispatchformatterserializereplystop.md)|Verbose|디스패처가 회신 메시지의 직렬화를 완료했습니다.|ServiceModel|  
|[3326 \- ClientFormatterSerializeRequestStart](../../../../../docs/framework/wcf/diagnostics/etw/3326-clientformatterserializerequeststart.md)|Verbose|클라이언트 요청 직렬화가 시작되었습니다.|ServiceModel|  
|[3327 \- ClientFormatterSerializeRequestStop](../../../../../docs/framework/wcf/diagnostics/etw/3327-clientformatterserializerequeststop.md)|Verbose|클라이언트에서 요청 메시지의 직렬화가 완료되었습니다.|ServiceModel|  
|[3328 \- ClientFormatterDeserializeReplyStart](../../../../../docs/framework/wcf/diagnostics/etw/3328-clientformatterdeserializereplystart.md)|Verbose|클라이언트에서 회신 메시지 역직렬화가 시작되었습니다.|ServiceModel|  
|[3329 \- ClientFormatterDeserializeReplyStop](../../../../../docs/framework/wcf/diagnostics/etw/3329-clientformatterdeserializereplystop.md)|Verbose|클라이언트에서 회신 메시지 역직렬화가 완료되었습니다.|ServiceModel|  
|[3330 \- SecurityNegotiationStart](../../../../../docs/framework/wcf/diagnostics/etw/3330-securitynegotiationstart.md)|Verbose|보안 협상이 시작되었습니다.|보안|  
|[3331 \- SecurityNegotiationStop](../../../../../docs/framework/wcf/diagnostics/etw/3331-securitynegotiationstop.md)|Verbose|보안 협상이 완료되었습니다.|보안|  
|[3332 \- SecurityTokenProviderOpened](../../../../../docs/framework/wcf/diagnostics/etw/3332-securitytokenprovideropened.md)|Verbose|SecurityTokenProvider 열기가 완료되었습니다.|보안|  
|[3333 \- OutgoingMessageSecured](../../../../../docs/framework/wcf/diagnostics/etw/3333-outgoingmessagesecured.md)|Verbose|보내는 메시지의 보안이 설정되었습니다.|보안|  
|[3334 \- IncomingMessageVerified](../../../../../docs/framework/wcf/diagnostics/etw/3334-incomingmessageverified.md)|Verbose|들어오는 메시지가 확인되었습니다.|보안 ServiceModel|  
|[3335 \- GetServiceInstanceStart](../../../../../docs/framework/wcf/diagnostics/etw/3335-getserviceinstancestart.md)|Verbose|서비스 인스턴스 검색이 시작되었습니다.|ServiceModel|  
|[3336 \- GetServiceInstanceStop](../../../../../docs/framework/wcf/diagnostics/etw/3336-getserviceinstancestop.md)|Verbose|서비스 인스턴스가 검색되었습니다.|ServiceModel|  
|[3337 \- ChannelReceiveStart](../../../../../docs/framework/wcf/diagnostics/etw/3337-channelreceivestart.md)|Verbose|ChannelHandlerId:%1 \- 메시지 수신 루프가 시작되었습니다.|채널|  
|[3338 \- ChannelReceiveStop](../../../../../docs/framework/wcf/diagnostics/etw/3338-channelreceivestop.md)|Verbose|ChannelHandlerId:%1 \- 메시지 수신 루프가 중지되었습니다.|채널|  
|[3339 \- ChannelFactoryCreated](../../../../../docs/framework/wcf/diagnostics/etw/3339-channelfactorycreated.md)|Verbose|ChannelFactory가 만들어졌습니다.|ServiceModel|  
|[3340 \- PipeConnectionAcceptStart](../../../../../docs/framework/wcf/diagnostics/etw/3340-pipeconnectionacceptstart.md)|Verbose|파이프 연결 수락이 %1에서 시작되었습니다.|채널|  
|[3341 \- PipeConnectionAcceptStop](../../../../../docs/framework/wcf/diagnostics/etw/3341-pipeconnectionacceptstop.md)|Verbose|파이프 연결이 수락되었습니다.|채널|  
|[3342 \- EstablishConnectionStart](../../../../../docs/framework/wcf/diagnostics/etw/3342-establishconnectionstart.md)|Verbose|%1에 대해 연결 설정이 시작되었습니다.|채널|  
|[3343 \- EstablishConnectionStop](../../../../../docs/framework/wcf/diagnostics/etw/3343-establishconnectionstop.md)|Verbose|연결이 설정되었습니다.|채널|  
|[3345 \- SessionPreambleUnderstood](../../../../../docs/framework/wcf/diagnostics/etw/3345-sessionpreambleunderstood.md)|Verbose|'%1'에 대한 세션 프리앰블이 확인되었습니다.|채널|  
|[3346 \- ConnectionReaderSendFault](../../../../../docs/framework/wcf/diagnostics/etw/3346-connectionreadersendfault.md)|오류|연결 판독기가 오류 '%1'을\(를\) 전송하고 있습니다.|채널|  
|[3347 \- SocketAcceptClosed](../../../../../docs/framework/wcf/diagnostics/etw/3347-socketacceptclosed.md)|Verbose|소켓 수락이 종료되었습니다.|TCP|  
|[3348 \- ServiceHostFaulted](../../../../../docs/framework/wcf/diagnostics/etw/3348-servicehostfaulted.md)|중요|서비스 호스트에 오류가 발생했습니다.|TCP|  
|[3349 \- ListenerOpenStart](../../../../../docs/framework/wcf/diagnostics/etw/3349-listeneropenstart.md)|Verbose|'%1'에 대한 리스너가 열려 있습니다.|채널|  
|[3350 \- ListenerOpenStop](../../../../../docs/framework/wcf/diagnostics/etw/3350-listeneropenstop.md)|Verbose|리스너 열기가 완료되었습니다.|채널|  
|[3351 \- ServerMaxPooledConnectionsQuotaReached](../../../../../docs/framework/wcf/diagnostics/etw/3351-servermaxpooledconnectionsquotareached.md)|Verbose|서버 최대 풀 연결 할당량에 도달했습니다.|할당량|  
|[3352 \- TcpConnectionTimedOut](../../../../../docs/framework/wcf/diagnostics/etw/3352-tcpconnectiontimedout.md)|오류|원격 주소 %2에 대한 SocketId:%1이\(가\) 시간 초과되었습니다.|TCP|  
|[3353 \- TcpConnectionResetError](../../../../../docs/framework/wcf/diagnostics/etw/3353-tcpconnectionreseterror.md)|경고|원격 주소 %2에 대한 SocketId:%1에 연결 재설정 오류가 발생했습니다.|TCP|  
|[3354 \- ServiceSecurityNegotiationCompleted](../../../../../docs/framework/wcf/diagnostics/etw/3354-servicesecuritynegotiationcompleted.md)|Verbose|서비스 보안 협상이 완료되었습니다.|보안|  
|[3355 \- SecurityNegotiationProcessingFailure](../../../../../docs/framework/wcf/diagnostics/etw/3355-securitynegotiationprocessingfailure.md)|오류|보안 협상을 처리하지 못했습니다.|보안|  
|[3356 \- SecurityIdentityVerificationSuccess](../../../../../docs/framework/wcf/diagnostics/etw/3356-securityidentityverificationsuccess.md)|Verbose|보안 확인에 성공했습니다.|보안|  
|[3357 \- SecurityIdentityVerificationFailure](../../../../../docs/framework/wcf/diagnostics/etw/3357-securityidentityverificationfailure.md)|오류|보안 확인에 실패했습니다.|보안|  
|[3358 \- PortSharingDuplicatedSocket](../../../../../docs/framework/wcf/diagnostics/etw/3358-portsharingduplicatedsocket.md)|Verbose|%1에 대해 소켓이 중복되었습니다.|ActivationServices|  
|[3359 \- SecurityImpersonationSuccess](../../../../../docs/framework/wcf/diagnostics/etw/3359-securityimpersonationsuccess.md)|Verbose|보안 가장에 성공했습니다.|보안|  
|[3360 \- SecurityImpersonationFailure](../../../../../docs/framework/wcf/diagnostics/etw/3360-securityimpersonationfailure.md)|경고|보안 가장에 실패했습니다.|보안|  
|[3361 \- HttpChannelRequestAborted](../../../../../docs/framework/wcf/diagnostics/etw/3361-httpchannelrequestaborted.md)|경고|Http 채널 요청이 중단되었습니다.|HTTP|  
|[3362 \- HttpChannelResponseAborted](../../../../../docs/framework/wcf/diagnostics/etw/3362-httpchannelresponseaborted.md)|경고|Http 채널 응답이 중단되었습니다.|HTTP|  
|[3363 \- HttpAuthFailed](../../../../../docs/framework/wcf/diagnostics/etw/3363-httpauthfailed.md)|경고|Http 인증이 실패했습니다.|HTTP|  
|[3364 \- SharedListenerProxyRegisterStart](../../../../../docs/framework/wcf/diagnostics/etw/3364-sharedlistenerproxyregisterstart.md)|Verbose|SharedListenerProxy 등록이 URI '%1'에 대해 시작되었습니다.|ActivationServices|  
|[3365 \- SharedListenerProxyRegisterStop](../../../../../docs/framework/wcf/diagnostics/etw/3365-sharedlistenerproxyregisterstop.md)|Verbose|SharedListenerProxy 등록이 중지됩니다.|ActivationServices|  
|[3366 \- SharedListenerProxyRegisterFailed](../../../../../docs/framework/wcf/diagnostics/etw/3366-sharedlistenerproxyregisterfailed.md)|오류|SharedListenerProxy 등록이 '%1' 상태로 실패했습니다.|ActivationServices|  
|[3367 \- ConnectionPoolPreambleFailed](../../../../../docs/framework/wcf/diagnostics/etw/3367-connectionpoolpreamblefailed.md)|오류|ConnectionPoolPreambleFailed가 발생했습니다.|채널|  
|[3368 \- SslOnInitiateUpgrade](../../../../../docs/framework/wcf/diagnostics/etw/3368-ssloninitiateupgrade.md)|Verbose|SslOnAcceptUpgradeStart|보안|  
|[3369 \- SslOnAcceptUpgrade](../../../../../docs/framework/wcf/diagnostics/etw/3369-sslonacceptupgrade.md)|Verbose|SslOnAcceptUpgradeStop|보안|  
|[3370 \- BinaryMessageEncodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3370-binarymessageencodingstart.md)|Verbose|BinaryMessageEncoder에서 메시지 인코딩이 시작되었습니다.|채널|  
|[3371 \- MtomMessageEncodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3371-mtommessageencodingstart.md)|Verbose|MtomMessageEncoder에서 메시지 인코딩이 시작되었습니다.|채널|  
|[3372 \- TextMessageEncodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3372-textmessageencodingstart.md)|Verbose|TextMessageEncoder에서 메시지 인코딩이 시작되었습니다.|채널|  
|[3373 \- BinaryMessageDecodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3373-binarymessagedecodingstart.md)|Verbose|BinaryMessageEncoder에서 메시지 디코딩이 시작되었습니다.|채널|  
|[3374 \- MtomMessageDecodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3374-mtommessagedecodingstart.md)|Verbose|MtomMessageEncoder에서 메시지 디코딩이 시작되었습니다.|채널|  
|[3375 \- TextMessageDecodingStart](../../../../../docs/framework/wcf/diagnostics/etw/3375-textmessagedecodingstart.md)|Verbose|TextMessageEncoder에서 메시지 디코딩이 시작되었습니다.|채널|  
|[3376 \- HttpResponseReceiveStart](../../../../../docs/framework/wcf/diagnostics/etw/3376-httpresponsereceivestart.md)|정보|Http 전송에서 메시지 수신이 시작되었습니다.|HTTP|  
|[3377 \- SocketReadStop](../../../../../docs/framework/wcf/diagnostics/etw/3377-socketreadstop.md)|Verbose|SocketId:%1이\(가\) '%3'에서 '%2'바이트를 읽었습니다.|TCP|  
|[3378 \- SocketAsyncReadStop](../../../../../docs/framework/wcf/diagnostics/etw/3378-socketasyncreadstop.md)|Verbose|SocketId:%1이\(가\) '%3'에서 '%2'바이트를 읽었습니다.|TCP|  
|[3379 \- SocketWriteStart](../../../../../docs/framework/wcf/diagnostics/etw/3379-socketwritestart.md)|Verbose|SocketId:%1에서 '%3'에 '%2'바이트를 쓰는 중입니다.|TCP|  
|[3380 \- SocketAsyncWriteStart](../../../../../docs/framework/wcf/diagnostics/etw/3380-socketasyncwritestart.md)|Verbose|SocketId:%1에서 '%3'에 '%2'바이트를 쓰는 중입니다.|TCP|  
|[3381 \- SequenceAcknowledgementSent](../../../../../docs/framework/wcf/diagnostics/etw/3381-sequenceacknowledgementsent.md)|Verbose|SessionId:%1 승인이 전송되었습니다.|채널|  
|[3382 \- ClientReliableSessionReconnect](../../../../../docs/framework/wcf/diagnostics/etw/3382-clientreliablesessionreconnect.md)|정보|SessionId:%1 다시 연결하는 중입니다.|채널|  
|[3383 \- ReliableSessionChannelFaulted](../../../../../docs/framework/wcf/diagnostics/etw/3383-reliablesessionchannelfaulted.md)|정보|SessionId:%1 오류가 발생했습니다.|채널|  
|[3384 \- WindowsStreamSecurityOnInitiateUpgrade](../../../../../docs/framework/wcf/diagnostics/etw/3384-windowsstreamsecurityoninitiateupgrade.md)|Verbose|WindowsStreamSecurity에서 보안 업그레이드를 시작하는 중입니다.|보안|  
|[3385 \- WindowsStreamSecurityOnAcceptUpgrade](../../../../../docs/framework/wcf/diagnostics/etw/3385-windowsstreamsecurityonacceptupgrade.md)|Verbose|Windows 스트리밍 보안 업그레이드를 수락합니다.|보안|  
|[3386 \- SocketConnectionAbort](../../../../../docs/framework/wcf/diagnostics/etw/3386-socketconnectionabort.md)|경고|SocketId:%1을\(를\) 중단하는 중입니다.|TCP|  
|[3388 \- HttpGetContextStart](../../../../../docs/framework/wcf/diagnostics/etw/3388-httpgetcontextstart.md)|Verbose|HttpGetContext가 시작됩니다.|HTTP|  
|[3389 \- ClientSendPreambleStart](../../../../../docs/framework/wcf/diagnostics/etw/3389-clientsendpreamblestart.md)|Verbose|클라이언트 전송 프리앰블이 시작됩니다.|채널|  
|[3390 \- ClientSendPreambleStop](../../../../../docs/framework/wcf/diagnostics/etw/3390-clientsendpreamblestop.md)|Verbose|클라이언트 전송 프리앰블이 중지됩니다.|채널|  
|[3391 \- HttpMessageReceiveFailed](../../../../../docs/framework/wcf/diagnostics/etw/3391-httpmessagereceivefailed.md)|경고|Http 메시지 수신이 실패했습니다.|HTTP|  
|[3392 \- TransactionScopeCreate](../../../../../docs/framework/wcf/diagnostics/etw/3392-transactionscopecreate.md)|정보|LocalIdentifier:'%1' 및 DistributedIdentifier:'%2'을\(를\) 사용하여 TransactionScope를 만드는 중입니다.|ServiceModel|  
|[3393 \- StreamedMessageReadByEncoder](../../../../../docs/framework/wcf/diagnostics/etw/3393-streamedmessagereadbyencoder.md)|정보|인코더가 스트리밍된 메시지를 읽었습니다.|채널|  
|[3394 \- StreamedMessageWrittenByEncoder](../../../../../docs/framework/wcf/diagnostics/etw/3394-streamedmessagewrittenbyencoder.md)|정보|인코더가 스트리밍된 메시지를 썼습니다.|채널|  
|[3395 \- MessageWrittenAsynchronouslyByEncoder](../../../../../docs/framework/wcf/diagnostics/etw/3395-messagewrittenasynchronouslybyencoder.md)|정보|인코더가 메시지를 비동기적으로 썼습니다.|채널|  
|[3396 \- BufferedAsyncWriteStart](../../../../../docs/framework/wcf/diagnostics/etw/3396-bufferedasyncwritestart.md)|정보|BufferId:%1에서 기본 스트림에 대한 '%2'바이트 쓰기를 완료했습니다.|채널|  
|[3397 \- BufferedAsyncWriteStop](../../../../../docs/framework/wcf/diagnostics/etw/3397-bufferedasyncwritestop.md)|정보|인코더가 메시지를 비동기적으로 썼습니다.|채널|  
|[3398 \- PipeSharedMemoryCreated](../../../../../docs/framework/wcf/diagnostics/etw/3398-pipesharedmemorycreated.md)|Verbose|파이프 공유 메모리가 '%1'에 만들어졌습니다.|채널|  
|[3399 \- NamedPipeCreated](../../../../../docs/framework/wcf/diagnostics/etw/3399-namedpipecreated.md)|Verbose|NamedPipe '%1'이\(가\) 만들어졌습니다.|채널|  
|[3401 \- SignatureVerificationStart](../../../../../docs/framework/wcf/diagnostics/etw/3401-signatureverificationstart.md)|Verbose|서명 확인이 시작되었습니다.|보안|  
|[3402 \- SignatureVerificationSuccess](../../../../../docs/framework/wcf/diagnostics/etw/3402-signatureverificationsuccess.md)|Verbose|서명 확인을 성공했습니다.|보안|  
|[3403 \- WrappedKeyDecryptionStart](../../../../../docs/framework/wcf/diagnostics/etw/3403-wrappedkeydecryptionstart.md)|Verbose|래핑된 키의 암호 해독이 시작되었습니다.|보안|  
|[3404 \- WrappedKeyDecryptionSuccess](../../../../../docs/framework/wcf/diagnostics/etw/3404-wrappedkeydecryptionsuccess.md)|Verbose|래핑된 키의 암호 해독에 성공했습니다.|보안|  
|[3405 \- EncryptedDataProcessingStart](../../../../../docs/framework/wcf/diagnostics/etw/3405-encrypteddataprocessingstart.md)|Verbose|암호화된 데이터 처리가 시작되었습니다.|보안|  
|[3406 \- EncryptedDataProcessingSuccess](../../../../../docs/framework/wcf/diagnostics/etw/3406-encrypteddataprocessingsuccess.md)|Verbose|암호화된 데이터 처리에 성공했습니다.|보안|  
|[3407 \- HttpPipelineProcessInboundRequestStart](../../../../../docs/framework/wcf/diagnostics/etw/3407-httppipelineprocessinboundrequeststart.md)|Verbose|Http 메시지 처리기가 인바운드 요청 처리를 시작했습니다.|HTTP|  
|[3408 \- HttpPipelineBeginProcessInboundRequestStart](../../../../../docs/framework/wcf/diagnostics/etw/3408-httppipelinebeginprocessinboundrequeststart.md)|Verbose|Http 메시지 처리기가 비동기 인바운드 요청 처리를 시작했습니다.|HTTP|  
|[3409 \- HttpPipelineProcessInboundRequestStop](../../../../../docs/framework/wcf/diagnostics/etw/3409-httppipelineprocessinboundrequeststop.md)|Verbose|Http 메시지 처리기가 인바운드 요청 처리를 완료했습니다.|HTTP|  
|[3410 \- HttpPipelineFaulted](../../../../../docs/framework/wcf/diagnostics/etw/3410-httppipelinefaulted.md)|경고|Http 메시지 처리기에서 오류가 발생했습니다.|HTTP|  
|[3411 \- HttpPipelineTimeoutException](../../../../../docs/framework/wcf/diagnostics/etw/3411-httppipelinetimeoutexception.md)|오류|WebSocket 연결 시간이 초과되었습니다.|HTTP|  
|[3412 \- HttpPipelineProcessResponseStart](../../../../../docs/framework/wcf/diagnostics/etw/3412-httppipelineprocessresponsestart.md)|Verbose|Http 메시지 처리기가 응답 처리를 시작했습니다.|HTTP|  
|[3413 \- HttpPipelineBeginProcessResponseStart](../../../../../docs/framework/wcf/diagnostics/etw/3413-httppipelinebeginprocessresponsestart.md)|Verbose|Http 메시지 처리기가 비동기 응답 처리를 시작했습니다.|HTTP|  
|[3414 \- HttpPipelineProcessResponseStop](../../../../../docs/framework/wcf/diagnostics/etw/3414-httppipelineprocessresponsestop.md)|Verbose|Http 메시지 처리기가 응답 처리를 완료했습니다.|HTTP|  
|[3415 \- WebSocketConnectionRequestSendStart](../../../../../docs/framework/wcf/diagnostics/etw/3415-websocketconnectionrequestsendstart.md)|Verbose|'%1'에 대한 WebSocket 연결 요청을 보내기 시작합니다.|HTTP|  
|[3416 \- WebSocketConnectionRequestSendStop](../../../../../docs/framework/wcf/diagnostics/etw/3416-websocketconnectionrequestsendstop.md)|Verbose|WebSocketId:%1 연결 요청을 보냈습니다.|HTTP|  
|[3417 \- WebSocketConnectionAcceptStart](../../../../../docs/framework/wcf/diagnostics/etw/3417-websocketconnectionacceptstart.md)|Verbose|WebSocket 연결 수락을 시작합니다.|HTTP|  
|[3418 \- WebSocketConnectionAccepted](../../../../../docs/framework/wcf/diagnostics/etw/3418-websocketconnectionaccepted.md)|Verbose|WebSocketId:%1 연결이 수락되었습니다.|HTTP|  
|[3419 \- WebSocketConnectionDeclined](../../../../../docs/framework/wcf/diagnostics/etw/3419-websocketconnectiondeclined.md)|오류|WebSocket 연결이 상태 코드 '%1'\(으\)로 거부되었습니다.|HTTP|  
|[3420 \- WebSocketConnectionFailed](../../../../../docs/framework/wcf/diagnostics/etw/3420-websocketconnectionfailed.md)|오류|WebSocket 연결 요청이 실패했습니다. '%1'|HTTP|  
|[3421 \- WebSocketConnectionAborted](../../../../../docs/framework/wcf/diagnostics/etw/3421-websocketconnectionaborted.md)|오류|WebSocketId:%1 연결이 중단되었습니다.|HTTP|  
|[3422 \- WebSocketAsyncWriteStart](../../../../../docs/framework/wcf/diagnostics/etw/3422-websocketasyncwritestart.md)|Verbose|WebSocketId:%1에서 '%3'에 '%2'바이트를 쓰는 중입니다.|HTTP|  
|[3423 \- WebSocketAsyncWriteStop](../../../../../docs/framework/wcf/diagnostics/etw/3423-websocketasyncwritestop.md)|Verbose|WebSocketId:%1에서 비동기 쓰기를 중지합니다.|HTTP|  
|[3424 \- WebSocketAsyncReadStart](../../../../../docs/framework/wcf/diagnostics/etw/3424-websocketasyncreadstart.md)|Verbose|WebSocketId:%1에서 읽기를 시작합니다.|HTTP|  
|[3425 \- WebSocketAsyncReadStop](../../../../../docs/framework/wcf/diagnostics/etw/3425-websocketasyncreadstop.md)|Verbose|WebSocketId:%1이\(가\) '%3'에서 '%2'바이트를 읽었습니다.|HTTP|  
|[3426 \- WebSocketCloseSent](../../../../../docs/framework/wcf/diagnostics/etw/3426-websocketclosesent.md)|Verbose|WebSocketId:%1에서 닫기 상태 '%3'\(으\)로 '%2'에 닫기 메시지를 보내는 중입니다.|HTTP|  
|[3427 \- WebSocketCloseOutputSent](../../../../../docs/framework/wcf/diagnostics/etw/3427-websocketcloseoutputsent.md)|Verbose|WebSocketId:%1에서 닫기 상태 '%3'\(으\)로 '%2'에 출력 닫기 메시지를 보내는 중입니다.|HTTP|  
|[3428 \- WebSocketConnectionClosed](../../../../../docs/framework/wcf/diagnostics/etw/3428-websocketconnectionclosed.md)|Verbose|WebSocketId:%1 연결이 닫혔습니다.|HTTP|  
|[3429 \- WebSocketCloseStatusReceived](../../../../../docs/framework/wcf/diagnostics/etw/3429-websocketclosestatusreceived.md)|Verbose|WebSocketId:%1 연결 닫기 메시지가 상태 '%2'\(으\)로 수신되었습니다.|HTTP|  
|[3430 \- WebSocketUseVersionFromClientWebSocketFactory](../../../../../docs/framework/wcf/diagnostics/etw/3430-websocketuseversionfromclientwebsocketfactory.md)|Verbose|클라이언트 WebSocket 팩터리 형식 '%1'에서 WebSocketVersion을 사용하는 중입니다.|HTTP|  
|[3431 \- WebSocketCreateClientWebSocketWithFactory](../../../../../docs/framework/wcf/diagnostics/etw/3431-websocketcreateclientwebsocketwithfactory.md)|Verbose|팩터리 형식이 '%1'인 클라이언트 WebSocket을 만드는 중입니다.|HTTP|  
|[3553 \- XamlServicesLoadStart](../../../../../docs/framework/wcf/diagnostics/etw/3553-xamlservicesloadstart.md)|정보|XamlServicesLoad 시작|WebHost|  
|[3554 \- XamlServicesLoadStop](../../../../../docs/framework/wcf/diagnostics/etw/3554-xamlservicesloadstop.md)|정보|XamlServicesLoad 중지|WebHost|  
|[3555 \- CreateWorkflowServiceHostStart](../../../../../docs/framework/wcf/diagnostics/etw/3555-createworkflowservicehoststart.md)|정보|CreateWorkflowServiceHost 시작|WebHost|  
|[3556 \- CreateWorkflowServiceHostStop](../../../../../docs/framework/wcf/diagnostics/etw/3556-createworkflowservicehoststop.md)|정보|CreateWorkflowServiceHost 중지|WebHost|  
|[3558 \- ServiceActivationStart](../../../../../docs/framework/wcf/diagnostics/etw/3558-serviceactivationstart.md)|정보|서비스 활성화 시작|WebHost|  
|[3559 \- ServiceActivationStop](../../../../../docs/framework/wcf/diagnostics/etw/3559-serviceactivationstop.md)|정보|서비스 활성화 중지|WebHost|  
|[3560 \- ServiceActivationAvailableMemory](../../../../../docs/framework/wcf/diagnostics/etw/3560-serviceactivationavailablememory.md)|Verbose|사용 가능한 메모리\(바이트\): %1|할당량|  
|[3800 \- RoutingServiceClosingClient](../../../../../docs/framework/wcf/diagnostics/etw/3800-routingserviceclosingclient.md)|정보|라우팅 서비스에서 클라이언트 '%1'을\(를\) 닫는 중입니다.|RoutingServices|  
|[3800 \- RoutingServiceClosingClient](../../../../../docs/framework/wcf/diagnostics/etw/3800-routingserviceclosingclient.md)|경고|라우팅 서비스 클라이언트 '%1'에 오류가 발생했습니다.|RoutingServices|  
|[3802 \- RoutingServiceCompletingOneWay](../../../../../docs/framework/wcf/diagnostics/etw/3802-routingservicecompletingoneway.md)|정보|라우팅 서비스 단방향 메시지를 완료하는 중입니다.|RoutingServices|  
|[3803 \- RoutingServiceProcessingFailure](../../../../../docs/framework/wcf/diagnostics/etw/3803-routingserviceprocessingfailure.md)|오류|주소가 '%1'인 끝점에서 메시지를 처리하는 동안 라우팅 서비스에 오류가 발생했습니다.|RoutingServices|  
|[3804 \- RoutingServiceCreatingClientForEndpoint](../../../../../docs/framework/wcf/diagnostics/etw/3804-routingservicecreatingclientforendpoint.md)|정보|라우팅 서비스에서 끝점 '%1'에 대한 클라이언트를 만드는 중입니다.|RoutingServices|  
|[3805 \- RoutingServiceDisplayConfig](../../../../../docs/framework/wcf/diagnostics/etw/3805-routingservicedisplayconfig.md)|Verbose|라우팅 서비스가 RouteOnHeadersOnly: %1, SoapProcessingEnabled: %2, EnsureOrderedDispatch: %3\(으\)로 구성되어 있습니다.|RoutingServices|  
|[3807 \- RoutingServiceCompletingTwoWay](../../../../../docs/framework/wcf/diagnostics/etw/3807-routingservicecompletingtwoway.md)|정보|라우팅 서비스 요청 회신 메시지를 완료하는 중입니다.|RoutingServices|  
|[3809 \- RoutingServiceMessageRoutedToEndpoints](../../../../../docs/framework/wcf/diagnostics/etw/3809-routingservicemessageroutedtoendpoints.md)|Verbose|라우팅 서비스에서 ID가 '%1'인 메시지를 %2 끝점 목록으로 라우팅했습니다.|RoutingServices|  
|[3810 \- RoutingServiceConfigurationApplied](../../../../../docs/framework/wcf/diagnostics/etw/3810-routingserviceconfigurationapplied.md)|정보|새 RoutingConfiguration이 라우팅 서비스에 적용되었습니다.|RoutingServices|  
|[3815 \- RoutingServiceProcessingMessage](../../../../../docs/framework/wcf/diagnostics/etw/3815-routingserviceprocessingmessage.md)|정보|라우팅 서비스에서 트랜잭션 %4에서 받은 ID: '%1', 동작: '%2', 인바운드 URL: '%3'인 메시지를 처리하는 중입니다.|RoutingServices|  
|[3816 \- RoutingServiceTransmittingMessage](../../../../../docs/framework/wcf/diagnostics/etw/3816-routingservicetransmittingmessage.md)|정보|라우팅 서비스에서 ID가 '%1'인 메시지\[작업 %2\]를 '%3'\(으\)로 전송하는 중입니다.|RoutingServices|  
|[3817 \- RoutingServiceCommittingTransaction](../../../../../docs/framework/wcf/diagnostics/etw/3817-routingservicecommittingtransaction.md)|정보|라우팅 서비스에서 ID가 '%1'인 트랜잭션을 커밋하는 중입니다.|RoutingServices|  
|[3818 \- RoutingServiceDuplexCallbackException](../../../../../docs/framework/wcf/diagnostics/etw/3818-routingserviceduplexcallbackexception.md)|오류|라우팅 서비스 구성 요소 %1에 중복 콜백 예외가 발생했습니다.|RoutingServices|  
|[3819 \- RoutingServiceMovedToBackup](../../../../../docs/framework/wcf/diagnostics/etw/3819-routingservicemovedtobackup.md)|정보|ID가 '%1'인 라우팅 서비스 메시지\[작업 %2\]를 백업 끝점 '%3'\(으\)로 이동했습니다.|RoutingServices|  
|[3820 \- RoutingServiceCreatingTransaction](../../../../../docs/framework/wcf/diagnostics/etw/3820-routingservicecreatingtransaction.md)|정보|라우팅 서비스에서 메시지를 처리하기 위해 ID가 '%1'인 새 트랜잭션을 만들었습니다.|RoutingServices|  
|[3821 \- RoutingServiceCloseFailed](../../../../../docs/framework/wcf/diagnostics/etw/3821-routingserviceclosefailed.md)|경고|아웃바운드 클라이언트 '%1'을\(를\) 닫는 동안 라우팅 서비스에 오류가 발생했습니다.|RoutingServices|  
|[3822 \- RoutingServiceSendingResponse](../../../../../docs/framework/wcf/diagnostics/etw/3822-routingservicesendingresponse.md)|정보|라우팅 서비스에서 동작이 '%1'인 응답 메시지를 다시 보내는 중입니다.|RoutingServices|  
|[3823 \- RoutingServiceSendingFaultResponse](../../../../../docs/framework/wcf/diagnostics/etw/3823-routingservicesendingfaultresponse.md)|경고|라우팅 서비스에서 동작이 '%1'인 오류 응답 메시지를 다시 보내는 중입니다.|RoutingServices|  
|[3824 \- RoutingServiceCompletingReceiveContext](../../../../../docs/framework/wcf/diagnostics/etw/3824-routingservicecompletingreceivecontext.md)|Verbose|라우팅 서비스에서 ID가 '%1'인 메시지에 대해 ReceiveContext.Complete를 호출하는 중입니다.|RoutingServices|  
|[3825 \- RoutingServiceAbandoningReceiveContext](../../../../../docs/framework/wcf/diagnostics/etw/3825-routingserviceabandoningreceivecontext.md)|경고|라우팅 서비스에서 ID가 '%1'인 메시지에 대해 ReceiveContext.Abandon을 호출하는 중입니다.|RoutingServices|  
|[3826 \- RoutingServiceUsingExistingTransaction](../../../../../docs/framework/wcf/diagnostics/etw/3826-routingserviceusingexistingtransaction.md)|Verbose|라우팅 서비스에서 기존 트랜잭션 '%1'을\(를\) 사용하여 메시지를 보냅니다.|RoutingServices|  
|[3827 \- RoutingServiceTransmitFailed](../../../../../docs/framework/wcf/diagnostics/etw/3827-routingservicetransmitfailed.md)|경고|'%1'\(으\)로 보내는 동안 라우팅 서비스에서 오류가 발생했습니다.|RoutingServices|  
|[3828 \- RoutingServiceFilterTableMatchStart](../../../../../docs/framework/wcf/diagnostics/etw/3828-routingservicefiltertablematchstart.md)|정보|라우팅 서비스 MessageFilterTable 일치 시작.|RoutingServices|  
|[3829 \- RoutingServiceFilterTableMatchStop](../../../../../docs/framework/wcf/diagnostics/etw/3829-routingservicefiltertablematchstop.md)|정보|라우팅 서비스 MessageFilterTable 일치 중지.|RoutingServices|  
|[3830 \- RoutingServiceAbortingChannel](../../../../../docs/framework/wcf/diagnostics/etw/3830-routingserviceabortingchannel.md)|Verbose|라우팅 서비스가 '%1' 채널에서 중단을 요청하고 있습니다.|RoutingServices|  
|[3831 \- RoutingServiceHandledException](../../../../../docs/framework/wcf/diagnostics/etw/3831-routingservicehandledexception.md)|Verbose|라우팅 서비스가 예외를 처리했습니다.|RoutingServices|  
|[3832 \- RoutingServiceTransmitSucceeded](../../../../../docs/framework/wcf/diagnostics/etw/3832-routingservicetransmitsucceeded.md)|정보|라우팅 서비스가 ID '%1인 메시지\[작업 %2\]를 '%3'\(으\)로 전송했습니다.|RoutingServices|  
|[4001 \- TransportListenerSessionsReceived](../../../../../docs/framework/wcf/diagnostics/etw/4001-transportlistenersessionsreceived.md)|Verbose|'%1'을\(를\) 통해 전송 리스너 세션이 수신되었습니다.|ActivationServices|  
|[4002 \- FailFastException](../../../../../docs/framework/wcf/diagnostics/etw/4002-failfastexception.md)|중요|FailFastException이 발생했습니다.|ActivationServices|  
|[4003 \- ServiceStartPipeError](../../../../../docs/framework/wcf/diagnostics/etw/4003-servicestartpipeerror.md)|오류|서비스 시작 파이프 오류가 발생했습니다.|ActivationServices|  
|[4008 \- DispatchSessionStart](../../../../../docs/framework/wcf/diagnostics/etw/4008-dispatchsessionstart.md)|Verbose|세션 디스패치가 시작되었습니다.|ActivationServices|  
|[4008 \- DispatchSessionStart](../../../../../docs/framework/wcf/diagnostics/etw/4008-dispatchsessionstart.md)|경고|보류 중인 항목이 '%2'개로 보류 중인 세션 큐가 꽉 차서 '%1'에 대한 세션을 디스패치하지 못했습니다.|ActivationServices|  
|[4011 \- MessageQueueRegisterStart](../../../../../docs/framework/wcf/diagnostics/etw/4011-messagequeueregisterstart.md)|Verbose|메시지 큐 등록이 시작됩니다.|ActivationServices|  
|[4012 \- MessageQueueRegisterAbort](../../../../../docs/framework/wcf/diagnostics/etw/4012-messagequeueregisterabort.md)|오류|URI '%2'에 대한 메시지 큐 등록이 중단되었습니다. 상태: '%1'.|ActivationServices|  
|[4013 \- MessageQueueUnregisterSucceeded](../../../../../docs/framework/wcf/diagnostics/etw/4013-messagequeueunregistersucceeded.md)|Verbose|URI '%1'에 대한 메시지 큐 등록을 취소했습니다.|ActivationServices|  
|[4014 \- MessageQueueRegisterFailed](../../../../../docs/framework/wcf/diagnostics/etw/4014-messagequeueregisterfailed.md)|오류|URI '%1'에 대한 메시지 큐를 등록하지 못했습니다. 상태: '%2'.|ActivationServices|  
|[4015 \- MessageQueueRegisterCompleted](../../../../../docs/framework/wcf/diagnostics/etw/4015-messagequeueregistercompleted.md)|정보|URI '%1'에 대한 메시지 큐 등록이 완료되었습니다.|ActivationServices|  
|[4016 \- MessageQueueDuplicatedSocketError](../../../../../docs/framework/wcf/diagnostics/etw/4016-messagequeueduplicatedsocketerror.md)|오류|메시지 큐로 소켓을 복제하지 못했습니다.|ActivationServices|  
|[4019 \- MessageQueueDuplicatedSocketComplete](../../../../../docs/framework/wcf/diagnostics/etw/4019-messagequeueduplicatedsocketcomplete.md)|Verbose|MessageQueueDuplicatedSocketComplete|ActivationServices|  
|[4020 \- TcpTransportListenerListeningStart](../../../../../docs/framework/wcf/diagnostics/etw/4020-tcptransportlistenerlisteningstart.md)|Verbose|TCP 전송 리스너가 URI '%1'에서 수신을 시작하는 중입니다.|ActivationServices|  
|[4021 \- TcpTransportListenerListeningStop](../../../../../docs/framework/wcf/diagnostics/etw/4021-tcptransportlistenerlisteningstop.md)|Verbose|TCP 전송 리스너가 수신 중입니다.|ActivationServices|  
|[4022 \- WebhostUnregisterProtocolFailed](../../../../../docs/framework/wcf/diagnostics/etw/4022-webhostunregisterprotocolfailed.md)|오류|오류 코드:%1|ActivationServices|  
|[4023 \- WasCloseAllListenerChannelInstancesCompleted](../../../../../docs/framework/wcf/diagnostics/etw/4023-wasclosealllistenerchannelinstancescompleted.md)|정보|WAS에서 모든 리스너 채널 인스턴스를 종료했습니다.|ActivationServices|  
|[4024 \- WasCloseAllListenerChannelInstancesFailed](../../../../../docs/framework/wcf/diagnostics/etw/4024-wasclosealllistenerchannelinstancesfailed.md)|오류|오류 코드:%1|ActivationServices|  
|[4025 \- OpenListenerChannelInstanceFailed](../../../../../docs/framework/wcf/diagnostics/etw/4025-openlistenerchannelinstancefailed.md)|오류|오류 코드:%1|ActivationServices|  
|[4026 \- WasConnected](../../../../../docs/framework/wcf/diagnostics/etw/4026-wasconnected.md)|Verbose|WAS가 연결되었습니다.|ActivationServices|  
|[4027 \- WasDisconnected](../../../../../docs/framework/wcf/diagnostics/etw/4027-wasdisconnected.md)|Verbose|WAS 연결이 해제되었습니다.|ActivationServices|  
|[4028 \- PipeTransportListenerListeningStart](../../../../../docs/framework/wcf/diagnostics/etw/4028-pipetransportlistenerlisteningstart.md)|Verbose|파이프 전송 리스너 수신이 URI %1에서 시작됩니다.|ActivationServices|  
|[4029 \- PipeTransportListenerListeningStop](../../../../../docs/framework/wcf/diagnostics/etw/4029-pipetransportlistenerlisteningstop.md)|Verbose|파이프 전송 리스너 수신이 중지됩니다.|ActivationServices|  
|[4030 \- DispatchSessionSuccess](../../../../../docs/framework/wcf/diagnostics/etw/4030-dispatchsessionsuccess.md)|정보|세션을 디스패치했습니다.|ActivationServices|  
|[4031 \- DispatchSessionFailed](../../../../../docs/framework/wcf/diagnostics/etw/4031-dispatchsessionfailed.md)|오류|세션을 디스패치하지 못했습니다.|ActivationServices|  
|[4032 \- WasConnectionTimedout](../../../../../docs/framework/wcf/diagnostics/etw/4032-wasconnectiontimedout.md)|중요|WAS 연결 시간이 초과되었습니다.|ActivationServices|  
|[4033 \- RoutingTableLookupStart](../../../../../docs/framework/wcf/diagnostics/etw/4033-routingtablelookupstart.md)|Verbose|라우팅 테이블 조회가 시작되었습니다.|ActivationServices|  
|[4034 \- RoutingTableLookupStop](../../../../../docs/framework/wcf/diagnostics/etw/4034-routingtablelookupstop.md)|Verbose|라우팅 테이블 조회가 완료되었습니다.|ActivationServices|  
|[4035 \- PendingSessionQueueRatio](../../../../../docs/framework/wcf/diagnostics/etw/4035-pendingsessionqueueratio.md)|Verbose|보류 중인 세션 큐 비율: %1\/%2|할당량|  
|[4600 \- MessageLogEventSizeExceeded](../../../../../docs/framework/wcf/diagnostics/etw/4600-messagelogeventsizeexceeded.md)|경고|ETW 이벤트 크기를 초과하므로 메시지를 기록할 수 없습니다.|WCFMessageLogging|  
|[4801 \- DiscoveryClientInClientChannelFailedToClose](../../../../../docs/framework/wcf/diagnostics/etw/4801-discoveryclientinclientchannelfailedtoclose.md)|경고|DiscoveryClientChannel 내에 만들어진 DiscoveryClient를 닫지 못해 중단했습니다.|검색|  
|[4802 \- DiscoveryClientProtocolExceptionSuppressed](../../../../../docs/framework/wcf/diagnostics/etw/4802-discoveryclientprotocolexceptionsuppressed.md)|정보|DiscoveryClient를 닫는 동안에는 ProtocolException이 표시되지 않습니다.  DiscoveryService가 DiscoveryClient에 응답을 계속 보내려고 하는 중일 수 있습니다.|검색|  
|[4803 \- DiscoveryClientReceivedMulticastSuppression](../../../../../docs/framework/wcf/diagnostics/etw/4803-discoveryclientreceivedmulticastsuppression.md)|정보|DiscoveryClient가 DiscoveryProxy로부터 멀티캐스트 비표시 오류\(Suppression\) 메시지를 받았습니다.|검색|  
|[4804 \- DiscoveryMessageReceivedAfterOperationCompleted](../../../../../docs/framework/wcf/diagnostics/etw/4804-discoverymessagereceivedafteroperationcompleted.md)|정보|해당 %3 작업이 완료되어 messageId\='%2'인 %1 메시지가 DiscoveryClient에서 삭제되었습니다.|검색|  
|[4805 \- DiscoveryMessageWithInvalidContent](../../../../../docs/framework/wcf/diagnostics/etw/4805-discoverymessagewithinvalidcontent.md)|경고|잘못된 내용이 있어 messageId\='%2'인 %1 메시지가 DiscoveryClient에서 삭제되었습니다.|검색|  
|[4806 \- DiscoveryMessageWithInvalidRelatesToOrOperationCompleted](../../../../../docs/framework/wcf/diagnostics/etw/4806-discoverymessagewithinvalidrelatestooroperationcompleted.md)|경고|해당 %4 작업이 완료되었거나 relatesTo 값이 잘못되어 messageId\='%2'이고 relatesTo\='%3'인 %1 메시지가 DiscoveryClient에서 삭제되었습니다.|검색|  
|[4807 \- DiscoveryMessageWithInvalidReplyTo](../../../../../docs/framework/wcf/diagnostics/etw/4807-discoverymessagewithinvalidreplyto.md)|경고|잘못된 ReplyTo 주소가 있어 messageId\='%1'인 검색 요청 메시지가 삭제되었습니다.|검색|  
|[4808 \- DiscoveryMessageWithNoContent](../../../../../docs/framework/wcf/diagnostics/etw/4808-discoverymessagewithnocontent.md)|경고|내용이 없어 %1 메시지가 삭제되었습니다.|검색|  
|[4809 \- DiscoveryMessageWithNullMessageId](../../../../../docs/framework/wcf/diagnostics/etw/4809-discoverymessagewithnullmessageid.md)|경고|메시지 머리글에 필요한 MessageId 속성이 없어 %1 메시지가 삭제되었습니다.|검색|  
|[4810 \- DiscoveryMessageWithNullMessageSequence](../../../../../docs/framework/wcf/diagnostics/etw/4810-discoverymessagewithnullmessagesequence.md)|경고|DiscoveryMessageSequence 속성이 없어 messageId\='%2'인 %1 메시지가 DiscoveryClient에서 삭제되었습니다.|검색|  
|[4811 \- DiscoveryMessageWithNullRelatesTo](../../../../../docs/framework/wcf/diagnostics/etw/4811-discoverymessagewithnullrelatesto.md)|경고|메시지 머리글에 필요한 RelatesTo 속성이 없어 messageId\='%2'인 %1 메시지가 DiscoveryClient에서 삭제되었습니다.|검색|  
|[4812 \- DiscoveryMessageWithNullReplyTo](../../../../../docs/framework/wcf/diagnostics/etw/4812-discoverymessagewithnullreplyto.md)|경고|ReplyTo 주소가 없어 messageId\='%1'인 검색 요청 메시지가 삭제되었습니다.|검색|  
|[4813 \- DuplicateDiscoveryMessage](../../../../../docs/framework/wcf/diagnostics/etw/4813-duplicatediscoverymessage.md)|경고|중복되어 messageId\='%2'인 %1 메시지가 삭제되었습니다.|검색|  
|[4814 \- EndpointDiscoverabilityDisabled](../../../../../docs/framework/wcf/diagnostics/etw/4814-endpointdiscoverabilitydisabled.md)|정보|EndpointAddress\='%1' 및 ListenUri\='%2'을\(를\) 사용하는 끝점의 검색 기능이 사용하지 않도록 설정되어 있습니다.|검색|  
|[4814 \- EndpointDiscoverabilityDisabled](../../../../../docs/framework/wcf/diagnostics/etw/4814-endpointdiscoverabilitydisabled.md)|정보|EndpointAddress\='%1' 및 ListenUri\='%2'을\(를\) 사용하는 끝점의 검색 기능이 사용하도록 설정되어 있습니다.|검색|  
|[4816 \- FindInitiatedInDiscoveryClientChannel](../../../../../docs/framework/wcf/diagnostics/etw/4816-findinitiatedindiscoveryclientchannel.md)|Verbose|끝점 검색을 위해 DiscoveryClientChannel에서 찾기 작업이 시작되었습니다.|검색|  
|[4817 \- InnerChannelCreationFailed](../../../../../docs/framework/wcf/diagnostics/etw/4817-innerchannelcreationfailed.md)|경고|DiscoveryClientChannel에서 EndpointAddress\='%1' 및 Via\='%2'을\(를\) 사용하는 검색된 끝점으로 채널을 만들지 못했습니다.  DiscoveryClientChannel은 이제 사용 가능한 다음 끝점으로 검색된 끝점을 사용하게 됩니다.|검색|  
|[4818 \- InnerChannelOpenFailed](../../../../../docs/framework/wcf/diagnostics/etw/4818-innerchannelopenfailed.md)|경고|DiscoveryClientChannel에서 EndpointAddress\='%1' 및 Via\='%2'을\(를\) 사용하는 검색된 끝점으로 채널을 열지 못했습니다.  DiscoveryClientChannel은 이제 사용 가능한 다음 끝점으로 검색된 끝점을 사용하게 됩니다.|검색|  
|[4819 \- InnerChannelOpenSucceeded](../../../../../docs/framework/wcf/diagnostics/etw/4819-innerchannelopensucceeded.md)|정보|DiscoveryClientChannel에서 끝점을 성공적으로 검색하고 이를 사용하여 채널을 열었습니다.  클라이언트가 EndpointAddress\='%1' 및 Via\='%2'을\(를\) 사용하여 서비스에 연결되었습니다.|검색|  
|[4820 \- SynchronizationContextReset](../../../../../docs/framework/wcf/diagnostics/etw/4820-synchronizationcontextreset.md)|정보|DiscoveryClientChannel에서 SynchronizationContext가 원래 값 %1\(으\)로 다시 설정되었습니다.|검색|  
|[4821 \- SynchronizationContextSetToNull](../../../../../docs/framework/wcf/diagnostics/etw/4821-synchronizationcontextsettonull.md)|정보|찾기 작업을 시작하기 전에 DiscoveryClientChannel에서 SynchronizationContext가 Null로 설정되었습니다.|검색|  
|[5001 \- DCSerializeWithSurrogateStart](../../../../../docs/framework/wcf/diagnostics/etw/5001-dcserializewithsurrogatestart.md)|Verbose|DataContract의 %1 serialize와 함께 서로게이트가 시작됩니다.|Serialization|  
|[5002 \- DCSerializeWithSurrogateStop](../../../../../docs/framework/wcf/diagnostics/etw/5002-dcserializewithsurrogatestop.md)|Verbose|DataContract serialize와 함께 서로게이트가 중지됩니다.|Serialization|  
|[5003 \- DCDeserializeWithSurrogateStart](../../../../../docs/framework/wcf/diagnostics/etw/5003-dcdeserializewithsurrogatestart.md)|Verbose|DataContract의 %1 deserialize와 함께 서로게이트가 시작됩니다.|Serialization|  
|[5004 \- DCDeserializeWithSurrogateStop](../../../../../docs/framework/wcf/diagnostics/etw/5004-dcdeserializewithsurrogatestop.md)|Verbose|DataContract deserialize와 함께 서로게이트가 중지됩니다.|Serialization|  
|[5005 \- ImportKnownTypesStart](../../../../../docs/framework/wcf/diagnostics/etw/5005-importknowntypesstart.md)|Verbose|ImportKnownTypes가 시작됩니다.|Serialization|  
|[5006 \- ImportKnownTypesStop](../../../../../docs/framework/wcf/diagnostics/etw/5006-importknowntypesstop.md)|Verbose|ImportKnownTypes가 중지됩니다.|Serialization|  
|[5007 \- DCResolverResolve](../../../../../docs/framework/wcf/diagnostics/etw/5007-dcresolverresolve.md)|Verbose|DataContract 확인자 확인 %1이\(가\) 시작됩니다.|Serialization|  
|[5008 \- DCGenWriterStart](../../../../../docs/framework/wcf/diagnostics/etw/5008-dcgenwriterstart.md)|Verbose|%2에 대한 DataContract %1 작성기 생성이 시작됩니다.|Serialization|  
|[5009 \- DCGenWriterStop](../../../../../docs/framework/wcf/diagnostics/etw/5009-dcgenwriterstop.md)|Verbose|DataContract 작성기 생성이 중지됩니다.|Serialization|  
|[5010 \- DCGenReaderStart](../../../../../docs/framework/wcf/diagnostics/etw/5010-dcgenreaderstart.md)|Verbose|%2에 대한 DataContract %1 판독기 생성이 시작됩니다.|Serialization|  
|[5011 \- DCGenReaderStop](../../../../../docs/framework/wcf/diagnostics/etw/5011-dcgenreaderstop.md)|Verbose|DataContract 생성이 중지됩니다.|Serialization|  
|[5012 \- DCJsonGenReaderStart](../../../../../docs/framework/wcf/diagnostics/etw/5012-dcjsongenreaderstart.md)|Verbose|%2에 대한 Json %1 판독기 생성이 시작됩니다.|Serialization|  
|[5013 \- DCJsonGenReaderStop](../../../../../docs/framework/wcf/diagnostics/etw/5013-dcjsongenreaderstop.md)|Verbose|Json 판독기 생성이 중지됩니다.|Serialization|  
|[5014 \- DCJsonGenWriterStart](../../../../../docs/framework/wcf/diagnostics/etw/5014-dcjsongenwriterstart.md)|Verbose|%2에 대한 Json %1 작성기 생성이 시작됩니다.|Serialization|  
|[5015 \- DCJsonGenWriterStop](../../../../../docs/framework/wcf/diagnostics/etw/5015-dcjsongenwriterstop.md)|Verbose|Json 작성기 생성이 중지됩니다.|Serialization|  
|[5016 \- GenXmlSerializableStart](../../../../../docs/framework/wcf/diagnostics/etw/5016-genxmlserializablestart.md)|Verbose|'%1'에 대해 serialize 가능한 Xml 생성이 시작됩니다.|Serialization|  
|[5017 \- GenXmlSerializableStop](../../../../../docs/framework/wcf/diagnostics/etw/5017-genxmlserializablestop.md)|Verbose|직렬화 가능한 Xml 생성이 중지됩니다.|Serialization|  
|[5203 \- JsonMessageDecodingStart](../../../../../docs/framework/wcf/diagnostics/etw/5203-jsonmessagedecodingstart.md)|Verbose|JsonMessageEncoder에서 메시지 디코딩이 시작되었습니다.|채널|  
|[5204 \- JsonMessageEncodingStart](../../../../../docs/framework/wcf/diagnostics/etw/5204-jsonmessageencodingstart.md)|Verbose|JsonMessageEncoder에서 메시지 인코딩이 시작되었습니다.|채널|  
|[5402 \- TokenValidationStarted](../../../../../docs/framework/wcf/diagnostics/etw/5402-tokenvalidationstarted.md)|Verbose|SecurityToken\('%1' 형식, ID '%2'\) 유효성 검사가 시작되었습니다.|보안|  
|[5403 \- TokenValidationSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5403-tokenvalidationsuccess.md)|Verbose|SecurityToken\('%1' 형식, ID '%2'\) 유효성 검사에 성공했습니다.|보안|  
|[5404 \- TokenValidationFailure](../../../../../docs/framework/wcf/diagnostics/etw/5404-tokenvalidationfailure.md)|오류|SecurityToken\('%1' 형식, ID '%2'\) 유효성 검사에 실패했습니다.  %3|보안|  
|[5405 \- GetIssuerNameSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5405-getissuernamesuccess.md)|Verbose|tokenid %2에서 발급자 이름 %1 검색에 성공했습니다.|보안|  
|[5406 \- GetIssuerNameFailure](../../../../../docs/framework/wcf/diagnostics/etw/5406-getissuernamefailure.md)|오류|tokenId:%1에서 발급자 이름 검색에 실패했습니다.|보안|  
|[5600 \- FederationMessageProcessingStarted](../../../../../docs/framework/wcf/diagnostics/etw/5600-federationmessageprocessingstarted.md)|Verbose|페더레이션 메시지 처리가 시작되었습니다.|보안|  
|[5601 \- FederationMessageProcessingSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5601-federationmessageprocessingsuccess.md)|Verbose|페더레이션 메시지 처리에 성공했습니다.|보안|  
|[5602 \- FederationMessageCreationStarted](../../../../../docs/framework/wcf/diagnostics/etw/5602-federationmessagecreationstarted.md)|Verbose|폼 게시에서 페더레이션 메시지를 만들기 시작했습니다.|보안|  
|[5603 \- FederationMessageCreationSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5603-federationmessagecreationsuccess.md)|Verbose|폼 게시에서 페더레이션 메시지 만들기에 성공했습니다.|보안|  
|[5604 \- SessionCookieReadingStarted](../../../../../docs/framework/wcf/diagnostics/etw/5604-sessioncookiereadingstarted.md)|Verbose|세션 쿠키에서 세션 토큰을 읽기 시작했습니다.|보안|  
|[5605 \- SessionCookieReadingSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5605-sessioncookiereadingsuccess.md)|Verbose|세션 쿠키에서 세션 토큰 읽기에 성공했습니다.|보안|  
|[5606 \- PrincipalSettingFromSessionTokenStarted](../../../../../docs/framework/wcf/diagnostics/etw/5606-principalsettingfromsessiontokenstarted.md)|Verbose|세션 토큰에서 보안 주체 설정이 시작되었습니다.|보안|  
|[5607 \- PrincipalSettingFromSessionTokenSuccess](../../../../../docs/framework/wcf/diagnostics/etw/5607-principalsettingfromsessiontokensuccess.md)|Verbose|세션 토큰에서 보안 주체 설정에 성공했습니다.|보안|  
|[57393 \- AppDomainUnload](../../../../../docs/framework/wcf/diagnostics/etw/57393-appdomainunload.md)|정보|AppDomain을 언로드하고 있습니다.  AppDomain.FriendlyName %1, ProcessName %2, ProcessId %3.|인프라|  
|[57394 \- HandledException](../../../../../docs/framework/wcf/diagnostics/etw/57394-handledexception.md)|정보|예외를 처리하는 중입니다.|인프라|  
|[57395 \- ShipAssertExceptionMessage](../../../../../docs/framework/wcf/diagnostics/etw/57395-shipassertexceptionmessage.md)|오류|예기치 않은 오류가 발생했습니다.  이 오류는 응용 프로그램에서 처리할 수 없습니다.  오류와 관련된 다음 메시지가 진단용으로 제공됩니다. %1.|인프라|  
|[57396 \- ThrowingException](../../../../../docs/framework/wcf/diagnostics/etw/57396-throwingexception.md)|경고|예외를 throw하고 있습니다.  원본: %1.|인프라|  
|[57397 \- UnhandledException](../../../../../docs/framework/wcf/diagnostics/etw/57397-unhandledexception.md)|중요|처리되지 않은 예외가 발생했습니다.|인프라|  
|[57399 \- TraceCodeEventLogCritical](../../../../../docs/framework/wcf/diagnostics/etw/57399-tracecodeeventlogcritical.md)|중요|EventLog에 기록합니다.|인프라|  
|[57400 \- TraceCodeEventLogError](../../../../../docs/framework/wcf/diagnostics/etw/57400-tracecodeeventlogerror.md)|오류|EventLog에 기록합니다.|인프라|  
|[57401 \- TraceCodeEventLogInfo](../../../../../docs/framework/wcf/diagnostics/etw/57401-tracecodeeventloginfo.md)|정보|EventLog에 기록합니다.|인프라|  
|[57402 \- TraceCodeEventLogVerbose](../../../../../docs/framework/wcf/diagnostics/etw/57402-tracecodeeventlogverbose.md)|Verbose|EventLog에 기록합니다.|인프라|  
|[57403 \- TraceCodeEventLogWarning](../../../../../docs/framework/wcf/diagnostics/etw/57403-tracecodeeventlogwarning.md)|경고|EventLog에 기록합니다.|인프라|  
|[57404 \- HandledExceptionWarning](../../../../../docs/framework/wcf/diagnostics/etw/57404-handledexceptionwarning.md)|경고|예외를 처리하는 중입니다.|인프라|  
|[62326 \- HttpHandlerPickedForUrl](../../../../../docs/framework/wcf/diagnostics/etw/62326-httphandlerpickedforurl.md)|정보|URL '%1'이\(가\) 루트 요소 형식 '%2'을\(를\) 사용하여 XAML 문서를 호스트합니다.  HTTP 처리기 형식 '%3'이\(가\) 이 URL에 대한 모든 요청에 서비스를 제공하도록 선택되었습니다.|WebHost|