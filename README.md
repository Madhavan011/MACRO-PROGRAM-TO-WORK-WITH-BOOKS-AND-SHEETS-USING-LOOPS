# MACRO-PROGRAM-TO-WORK-WITH-BOOKS-AND-SHEETS-USING-LOOPS
Sub Button2_Click() 

Dim book As Workbook, sheet As Worksheet, text As StringFor Each book In Workbooks 

text = text & "Workbook: " & book.Name & vbNewLine & "Worksheets: "& vbNewLine 

For Each sheet In book.Worksheets 

text = text & sheet.Name & vbNewLineNext sheet 

text = text & vbNewLine Next book 

MsgBox text 

End Sub
