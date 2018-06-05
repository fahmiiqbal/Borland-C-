# Borland-C-
Private Sub Command1_Click()
p = MsgBox("Anda Mau Keluar", vbQuestion + vbOKCancel, "info")
If p = vbOK Then
End
End If
End Sub

Private Sub do_Click()
List1.Clear
i = 1
Do Until i > 5
List1.AddItem (i)
i = i + 1
Loop
End Sub

Private Sub Form_Load()
For i = 1 To 31
Me.tgl.AddItem (Str(i))
Next i
For i = 1 To 12
Me.bln.AddItem (MonthName(i))
Next i
For i = 1990 To Year(Now)
Me.thn.AddItem (Str(i))
Next i
End Sub

