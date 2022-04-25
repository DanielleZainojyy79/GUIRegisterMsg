# GUIRegisterMsg
GUICtrlListView_AutoResizeColumn($hWnd, $hListView)     Local Static $iRLV_Flag = 0     Local $iColCount, $aiGetSize, $iWidth      If Not $iRLV_Flag Then         Global $__hARC_ListView = $hListView         $iRLV_Flag = 1         GUIRegisterMsg($WM_SIZING, "_GUICtrlListView_AutoResizeColumn")         GUIRegisterMsg($WM_SIZE, "_GUICtrlListView_AutoResizeColumn")
