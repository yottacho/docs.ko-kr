---
title: "&lt;ws2007FederationHttpBinding&gt;의 &lt;security&gt; 요소 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 826219b4-3a16-45fc-832d-0cd7cbbd3b84
caps.latest.revision: 10
author: "BrucePerlerMS"
ms.author: "bruceper"
manager: "mbaldwin"
caps.handback.revision: 10
---
# &lt;ws2007FederationHttpBinding&gt;의 &lt;security&gt; 요소
[\<ws2007FederationHttpBinding\>](../../../../../docs/framework/configure-apps/file-schema/wcf/ws2007federationhttpbinding.md) 요소의 보안 설정을 정의합니다.  
  
## 구문  
  
```  
  
<ws2007FederationBinding>  
    <binding >  
        <security mode="None/Message/TransportWithMessageCredential">  
           <message negotiateServiceCredential="Boolean"  
                algorithmSuite="Basic128/Basic192/Basic256/Basic128Rsa15/ Basic256Rsa15/TripleDes/TripleDesRsa15/Basic128Sha256/Basic192Sha256/TripleDesSha256/Basic128Sha256Rsa15/Basic192Sha256Rsa15/Basic256Sha256Rsa15/TripleDesSha256Rsa15"  
                defaultProtectionLevel="none/sign/EncryptAndSign"   
                issuedTokenType="string"   
                issuedKeyType="SymmetricKey/PublicKey"  
           </message>  
        </security>  
    </binding>  
</ws2007FederationBinding>  
```  
  
## 특성 및 요소  
 다음 단원에서는 특성, 자식 요소 및 부모 요소에 대해 설명합니다.  
  
### 특성  
  
|특성|설명|  
|--------|--------|  
|`mode`|선택 사항입니다.  적용되는 보안 형식을 지정합니다.  기본값은 `Message`입니다.  이 특성은 <xref:System.ServiceModel.WSFederationHttpSecurityMode> 형식입니다.|  
  
## mode 특성  
  
|값|설명|  
|-------|--------|  
|없음|SOAP 메시지의 경우 전송 중에는 안전하지 않습니다.|  
|메시지|SOAP 메시지 보안을 사용하여 무결성, 기밀성, 서버 인증 및 클라이언트 인증을 제공합니다.  기본적으로 본문에는 암호화 및 서명이 수행됩니다.  인증서를 사용하여 서비스를 구성해야 합니다.  클라이언트 인증은 보안 토큰 서비스가 클라이언트에 발급한 토큰에 따라 수행됩니다.|  
|TransportWithMessageCredential|HTTPS를 사용하여 무결성, 기밀성 및 서버 인증을 제공합니다.  인증서를 사용하여 서비스를 구성해야 합니다.  클라이언트 인증은 SOAP 메시지 보안을 통해 제공되며 보안 토큰 서비스가 클라이언트에 발급한 토큰에 따라 수행됩니다.|  
  
### 자식 요소  
  
|요소|설명|  
|--------|--------|  
|[\<message\>](../../../../../docs/framework/configure-apps/file-schema/wcf/message-of-ws2007httpbinding.md)|메시지 수준 보안 설정을 정의합니다.  이 요소는 <xref:System.ServiceModel.Configuration.FederatedMessageSecurityOverHttpElement> 형식입니다.|  
  
### 부모 요소  
  
|요소|설명|  
|--------|--------|  
|[\<binding\>](../../../../../docs/framework/misc/binding.md)|[\<wsDualHttpBinding\>](../../../../../docs/framework/configure-apps/file-schema/wcf/wsdualhttpbinding.md)의 모든 바인딩 기능을 정의합니다.|  
  
## 참고 항목  
 <xref:System.ServiceModel.WSFederationHttpSecurity>   
 <xref:System.ServiceModel.WSFederationHttpBinding.Security%2A>   
 <xref:System.ServiceModel.Configuration.WSFederationHttpBindingElement.Security%2A>   
 <xref:System.ServiceModel.Configuration.WSFederationHttpSecurityElement>   
 [방법: WSFederationHttpBinding 만들기](../../../../../docs/framework/wcf/feature-details/how-to-create-a-wsfederationhttpbinding.md)   
 [서비스 및 클라이언트에 보안 설정](../../../../../docs/framework/wcf/feature-details/securing-services-and-clients.md)   
 [자격 증명 형식 선택](../../../../../docs/framework/wcf/feature-details/selecting-a-credential-type.md)   
 [바인딩](../../../../../docs/framework/wcf/bindings.md)   
 [시스템 제공 바인딩 구성](../../../../../docs/framework/wcf/feature-details/configuring-system-provided-bindings.md)   
 [Using Bindings to Configure Windows Communication Foundation Services and Clients](http://msdn.microsoft.com/ko-kr/bd8b277b-932f-472f-a42a-b02bb5257dfb)   
 [\<binding\>](../../../../../docs/framework/misc/binding.md)