---
title: '방법: ScrollChanged 이벤트 처리'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- ScrollViewer control [WPF], raising ScrollChanged events
- ScrollChanged events [WPF]
ms.assetid: 42c695d8-ee28-49d4-80fd-fc71e9be7f29
ms.openlocfilehash: da7c1d1174e3264b21763177487ebcb75a4b3192
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
ms.locfileid: "33552703"
---
# <a name="how-to-handle-the-scrollchanged-event"></a>방법: ScrollChanged 이벤트 처리
## <a name="example"></a>예제  
 처리 하는 방법을 보여 주는이 예제는 <xref:System.Windows.Controls.ScrollViewer.ScrollChanged> 의 이벤트는 <xref:System.Windows.Controls.ScrollViewer>합니다.  
  
 A <xref:System.Windows.Documents.FlowDocument> 요소 <xref:System.Windows.Documents.Paragraph> 파트에 정의 된 [!INCLUDE[TLA2#tla_xaml](../../../../includes/tla2sharptla-xaml-md.md)]합니다. 경우는 <xref:System.Windows.Controls.ScrollViewer.ScrollChanged> 사용자 상호 작용으로 인해 이벤트가 발생할 처리기가 호출 되 고 텍스트에 기록 됩니다는 <xref:System.Windows.Controls.TextBlock> 이벤트가 발생 했음을 나타내는입니다.  
  
 [!code-xaml[scrollchangedeventargsLayout#1](../../../../samples/snippets/csharp/VS_Snippets_Wpf/scrollchangedeventargsLayout/CSharp/Window1.xaml#1)]  
[!code-xaml[scrollchangedeventargsLayout#2](../../../../samples/snippets/csharp/VS_Snippets_Wpf/scrollchangedeventargsLayout/CSharp/Window1.xaml#2)]  
  
 [!code-csharp[scrollchangedeventargsLayout#3](../../../../samples/snippets/csharp/VS_Snippets_Wpf/scrollchangedeventargsLayout/CSharp/Window1.xaml.cs#3)]
 [!code-vb[scrollchangedeventargsLayout#3](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/scrollchangedeventargsLayout/VisualBasic/Window1.xaml.vb#3)]  
  
## <a name="see-also"></a>참고 항목  
 <xref:System.Windows.Controls.ScrollViewer>  
 <xref:System.Windows.Controls.ScrollViewer.ScrollChanged>  
 <xref:System.Windows.Controls.ScrollChangedEventHandler>  
 <xref:System.Windows.Controls.ScrollChangedEventArgs>
