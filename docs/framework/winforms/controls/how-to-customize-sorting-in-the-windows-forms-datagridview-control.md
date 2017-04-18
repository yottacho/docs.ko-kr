---
title: "방법: Windows Forms DataGridView 컨트롤에서 정렬 사용자 지정 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-winforms"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "jsharp"
helpviewer_keywords: 
  - "데이터 표, 정렬 사용자 지정"
  - "DataGridView 컨트롤[Windows Forms], 정렬"
  - "정렬, DataGridView 컨트롤"
ms.assetid: 92fb5c14-afab-4cf5-a97e-924fd9cb99f5
caps.latest.revision: 12
author: "dotnet-bot"
ms.author: "dotnetcontent"
manager: "wpickett"
caps.handback.revision: 12
---
# 방법: Windows Forms DataGridView 컨트롤에서 정렬 사용자 지정
<xref:System.Windows.Forms.DataGridView> 컨트롤은 자동 정렬을 제공하지만 필요에 따라 정렬 작업을 사용자 지정해야 할 수도 있습니다.  예를 들어 프로그래밍 방식의 정렬을 사용하여 대체 UI\(사용자 인터페이스\)를 만들 수 있습니다.  또는 다중 열 정렬과 같은 정렬 유연성 향상을 위해 <xref:System.Windows.Forms.DataGridView.SortCompare> 이벤트를 처리하거나 <xref:System.Windows.Forms.DataGridView.Sort%2A> 메서드의 `Sort(IComparer)` 오버로드를 호출할 수 있습니다.  
  
 다음 코드 예제에서는 사용자 지정 정렬에 대한 이 세 가지 접근 방식을 보여 줍니다.  자세한 내용은 [Windows Forms DataGridView 컨트롤의 열 정렬 모드](../../../../docs/framework/winforms/controls/column-sort-modes-in-the-windows-forms-datagridview-control.md)를 참조하세요.  
  
## 프로그래밍 방식 정렬  
 다음 코드 예제에서는 <xref:System.Windows.Forms.DataGridView.SortOrder%2A> 및 <xref:System.Windows.Forms.DataGridView.SortedColumn%2A> 속성을 사용하여 정렬 방향을 결정하고 <xref:System.Windows.Forms.DataGridViewColumnHeaderCell.SortGlyphDirection%2A> 속성을 사용하여 정렬 문자를 수동으로 설정하는 프로그래밍 방식 정렬을 보여 줍니다.  <xref:System.Windows.Forms.DataGridView.Sort%2A> 메서드의 `Sort(DataGridViewColumn,ListSortDirection)` 오버로드는 단일 열의 데이터만 정렬하는 데 사용됩니다.  
  
 [!code-csharp[System.Windows.Forms.DataGridViewProgrammaticSort#00](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewProgrammaticSort/CS/form1.cs#00)]
 [!code-vb[System.Windows.Forms.DataGridViewProgrammaticSort#00](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewProgrammaticSort/VB/form1.vb#00)]  
  
## SortCompare 이벤트를 사용한 사용자 지정 정렬  
 다음 코드 예제에서는 <xref:System.Windows.Forms.DataGridView.SortCompare> 이벤트 처리기를 사용한 사용자 지정 정렬을 보여 줍니다.  선택한 <xref:System.Windows.Forms.DataGridViewColumn>이 정렬되고, 열에 중복 값이 있는 경우 ID 열을 사용하여 최종 순서를 결정합니다.  
  
 [!code-csharp[System.Windows.Forms.DataGridView.SortCompare#00](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.DataGridView.SortCompare/CS/form1.cs#00)]
 [!code-vb[System.Windows.Forms.DataGridView.SortCompare#00](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.DataGridView.SortCompare/VB/form1.vb#00)]  
  
## IComparer 인터페이스를 사용한 사용자 지정 정렬  
 다음 코드 예제에서는 <xref:System.Collections.IComparer> 인터페이스 구현을 받아서 다중 열 정렬을 수행하는 <xref:System.Windows.Forms.DataGridView.Sort%2A> 메서드의 `Sort(IComparer)` 오버로드를 사용한 사용자 지정 정렬을 보여 줍니다.  
  
 [!code-csharp[System.Windows.Forms.DataGridViewIComparerSort#00](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewIComparerSort/CS/form1.cs#00)]
 [!code-vb[System.Windows.Forms.DataGridViewIComparerSort#00](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewIComparerSort/VB/form1.vb#00)]  
  
## 코드 컴파일  
 이러한 예제에는 다음이 필요합니다.  
  
-   System, System.Drawing 및 System.Windows.Forms 어셈블리에 대한 참조  
  
 명령줄에서 [!INCLUDE[vbprvb](../../../../includes/vbprvb-md.md)] 또는 [!INCLUDE[csprcs](../../../../includes/csprcs-md.md)]용으로 이들 예제를 빌드하는 방법에 대한 자세한 내용은 [명령줄에서 빌드](../Topic/Building%20from%20the%20Command%20Line%20\(Visual%20Basic\).md) 또는 [csc.exe를 사용한 명령줄 빌드](../../../../ocs/csharp/language-reference/compiler-options/command-line-building-with-csc-exe.md)를 참조하세요.  [!INCLUDE[vsprvs](../../../../includes/vsprvs-md.md)]에서 코드를 새 프로젝트에 붙여넣어 이 예제를 빌드할 수도 있습니다.  [방법: Visual Studio를 사용하여 전체 Windows Forms 코드 예제 컴파일 및 실행](http://msdn.microsoft.com/library/Bb129228\(v=vs.110\))을 참조하세요.  
  
## 참고 항목  
 <xref:System.Windows.Forms.DataGridView>   
 [Windows Forms DataGridView 컨트롤의 데이터 정렬](../../../../docs/framework/winforms/controls/sorting-data-in-the-windows-forms-datagridview-control.md)   
 [Windows Forms DataGridView 컨트롤의 열 정렬 모드](../../../../docs/framework/winforms/controls/column-sort-modes-in-the-windows-forms-datagridview-control.md)   
 [방법: Windows Forms DataGridView 컨트롤의 열 정렬 모드 설정](../../../../docs/framework/winforms/controls/set-the-sort-modes-for-columns-wf-datagridview-control.md)