---
title: "Basic Serialization 기술 샘플 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 9d824e16-08d1-4a36-bc7f-2388c1f75f34
caps.latest.revision: 9
author: "Erikre"
ms.author: "erikre"
manager: "erikre"
caps.handback.revision: 6
---
# Basic Serialization 기술 샘플
[샘플 다운로드](http://download.microsoft.com/download/4/7/B/47B2164C-E780-4B10-8DE4-2CB5B886E0A6/Technologies/Serialization/Runtime%20Serialization/Basic.zip.exe)  
  
 이 샘플에서는 메모리에서 개체 그래프를 스트림으로 serialize하는 공용 언어 런타임의 기능을 보여 줍니다.이 샘플에서는 serialization을 위해 <xref:System.Runtime.Serialization.Formatters.Soap.SoapFormatter> 또는 <xref:System.Runtime.Serialization.Formatters.Binary.BinaryFormatter>를 사용할 수 있으며,데이터가 채워진 연결된 목록을 파일 스트림으로 serialize하거나 파일 스트림에서 deserialize합니다.두 경우 모두 결과를 확인할 수 있도록 목록이 화면에 표시됩니다.연결된 목록은 이 샘플에서 정의한 형식인 `LinkedList` 형식입니다.  
  
 serialization에 대한 자세한 내용은 build.proj 파일 및 소스 코드의 주석을 참조하십시오.  
  
### 명령 프롬프트를 사용하여 샘플을 빌드하려면  
  
1.  명령 프롬프트를 사용하여 Technologies\\Serialization\\Runtime Serialization\\Basic 디렉터리 아래의 언어별 하위 디렉터리 중 하나로 이동합니다.  
  
2.  선택한 프로그래밍 언어에 따라 **msbuild SerializationCS.sln**, **msbuild SerializationJSL.sln** 또는 **msbuild SerializationVB.sln**을 명령줄에 입력합니다.  
  
### Visual Studio를 사용하여 샘플을 빌드하려면  
  
1.  [!INCLUDE[fileExplorer](../../../includes/fileexplorer-md.md)]를 열고 샘플에 대한 언어별 하위 디렉터리 중 하나로 이동합니다.  
  
2.  선택한 프로그래밍 언어에 따라 RemotingIPCCS.sln, RemotingIPCJSL.sln 또는 RemotingIPCVB.sln 파일의 아이콘을 두 번 클릭하여 Visual Studio에서 파일을 엽니다.  
  
3.  **빌드** 메뉴에서 **솔루션 빌드**를 선택합니다.  
  
 샘플 응용 프로그램이 기본 \\bin 또는 \\bin\\Debug 하위 디렉터리에 빌드됩니다.  
  
### 이 샘플을 실행하려면  
  
1.  빌드된 실행 파일이 있는 디렉터리로 이동합니다.  
  
2.  원하는 매개 변수 값과 함께 **Serialization.exe**를 명령줄에 입력합니다.  
  
    > [!NOTE]
    >  이 샘플은 콘솔 응용 프로그램을 빌드합니다.출력을 보려면 명령 프롬프트를 사용하여 시작해야 합니다.  
  
## 설명  
 이 샘플 응용 프로그램에서는 실행할 테스트를 지정하는 명령줄 매개 변수를 받습니다.노드가 10개인 목록을 SOAP 포맷터를 사용하여 **Test.xml** 파일로 serialize하려면 **sx Test.xml 10** 매개 변수를 사용합니다.  
  
 예를 들면 다음과 같습니다.  
  
 **Serialize.exe \-sx Test.xml 10**  
  
 이전 샘플의 **Test.xml** 파일을 deserialize하려면 매개 변수로 **dx Test.xml**을 사용합니다.  
  
 예를 들면 다음과 같습니다.  
  
 **Serialize.exe \-dx Test.xml**  
  
 위의 두 예제에서 명령줄 스위치에 있는 "x"는 XML SOAP serialization을 사용하도록 지정하는 데 사용됩니다.이진 serialization을 사용하려면 대신 "b"를 사용합니다.매우 많은 노드를 serialize하는 경우에는 콘솔 출력을 파일로 리디렉션하는 것이 좋습니다.  
  
 예를 들면 다음과 같습니다.  
  
 **Serialize.exe \-sb Test.bin 10000 \>somefile.txt**  
  
 이 샘플에 사용된 클래스 및 기술이 아래에 간략하게 설명되어 있습니다.  
  
-   런타임 serialization  
  
    -   <xref:System.Runtime.Serialization.Formatters.Binary.BinaryFormatter> 또는 <xref:System.Runtime.Serialization.Formatters.Soap.SoapFormatter> 개체를 참조하기 위해 <xref:System.Runtime.Serialization.IFormatter>가 사용됩니다.  
  
    -   연결된 목록을 스트림에 이진 형식으로 serialize하기 위해 <xref:System.Runtime.Serialization.Formatters.Binary.BinaryFormatter>가 사용됩니다.이진 포맷터는 <xref:System.Runtime.Serialization.Formatters.Binary.BinaryFormatter> 형식에서만 인식할 수 있는 형식을 사용하지만,데이터가 간결해지는 장점이 있습니다.  
  
    -   연결된 목록을 스트림에 SOAP 형식으로 serialize하기 위해 <xref:System.Runtime.Serialization.Formatters.Soap.SoapFormatter>가 사용됩니다.SOAP는 표준 형식입니다.  
  
-   스트림 I\/O  
  
    -   serialize 및 deserialize를 위해 <xref:System.IO.Stream>이 사용됩니다.이 샘플에서 사용되는 특정 스트림 형식은 <xref:System.IO.FileStream> 형식입니다.그러나 serialization에는 <xref:System.IO.Stream>에서 파생되는 모든 형식을 사용할 수 있습니다.  
  
    -   디스크에 파일을 생성하고 디스크의 파일을 읽기 위한 <xref:System.IO.FileStream> 개체를 만들기 위해 <xref:System.IO.File>이 사용됩니다.  
  
    -   연결된 목록을 serialize 및 deserialize하기 위해 <xref:System.IO.FileStream>이 사용됩니다.  
  
## 참고 항목  
 [BinaryFormatter 클래스](frlrfSystemRuntimeSerializationFormattersBinaryBinaryFormatterClassTopic)   
 [File 클래스](frlrfSystemIOFileClassTopic)   
 [FileStream 클래스](frlrfSystemIOFileStreamClassTopic)   
 [IFormatter 인터페이스](frlrfSystemRuntimeSerializationIFormatterClassTopic)   
 [Random 클래스](https://msdn.microsoft.com/en-us/library/system.random.aspx)   
 [SerializableAttribute 특성](frlrfSystemSerializableAttributeClassTopic)   
 [SoapFormatter 클래스](frlrfSystemRuntimeSerializationFormattersSoapSoapFormatterClassTopic)   
 [Stream 클래스](frlrfSystemIOStreamClassTopic)   
 [System.IO 네임스페이스](https://msdn.microsoft.com/en-us/library/system.io.aspx)   
 [System.Runtime.Serialization 네임스페이스](frlrfSystemRuntimeSerialization)   
 [System. Xml.Serialization 네임스페이스](frlrfSystemXmlSerialization)   
 [기본 Serialization](../../../docs/framework/serialization/basic-serialization.md)   
 [이진 Serialization](../../../docs/framework/serialization/binary-serialization.md)   
 [특성을 사용하여 XML Serialization 제어](../../../docs/framework/serialization/controlling-xml-serialization-using-attributes.md)   
 [XML Serialization 소개](../../../docs/framework/serialization/introducing-xml-serialization.md)   
 [Serialization](../../../docs/framework/serialization/index.md)   
 [SOAP Service](http://msdn.microsoft.com/ko-kr/2051c992-28d1-499e-961f-17e9b675cec9)   
 [XML 및 SOAP Serialization](../../../docs/framework/serialization/xml-and-soap-serialization.md)